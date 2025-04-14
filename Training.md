# Training Instructions


* Initial training 


        deepspeed --master_port=29504 --num_gpus=4 train_ds_with_videogptplus.py \
            --videogptplus_path="./checkpoints_hf/MBZUAI/VideoGPT-plus_Phi3-mini-4k/mvbench" \
            --vision_tower="./OpenGVLab/InternVideo2-Stage2_1B-224p-f4/InternVideo2-stage2_1b-224p-f4.pt" \
            --image_vision_tower="openai/clip-vit-large-patch14-336" \
            --dataset_dir='./dataset' \
            --video_dataset_dir='./video_dataset' \
            --sam_pretrained_path="./checkpoints/sam2/sam2_hiera_large.pt" \
            --exp_name="sam2_videogptplusphi3" \
            --logs_base_dir "./runs/logs" \
            --ckpt_base_dir "./runs/ckpts" \
            --dataset="sem_seg||refer_seg||vqa||reason_seg||grandf||refer_vos||mevis||vidstg||video_vqa" \
            --sample_rates_for_datasets="9,3,3,1,1,10,10,10,10,10" \
            --train_mask_decoder=False \
            --tune_mm_mlp_adapter=True \
            --use_sam_version='v2' \
            --precision='fp16' \
            --num_frames_for_sam=8 \
            --batch_size=1 \
            --grad_accumulation_steps=10 \
            --epochs=20 \
            --auto_resume

* Finetuning with video-GCG data

        deepspeed --master_port=29504 --num_gpus=4 train_ds_with_videogptplus.py \
            --videogptplus_path="./checkpoints_hf/MBZUAI/VideoGPT-plus_Phi3-mini-4k/mvbench" \
            --vision_tower="./OpenGVLab/InternVideo2-Stage2_1B-224p-f4/InternVideo2-stage2_1b-224p-f4.pt" \
            --image_vision_tower="openai/clip-vit-large-patch14-336" \
            --dataset_dir='./dataset' \
            --video_dataset_dir='./video_dataset' \
            --sam_pretrained_path="./checkpoints/sam2/sam2_hiera_large.pt" \
            --exp_name="sam2_videogptplusphi3" \
            --logs_base_dir "./runs/logs" \
            --ckpt_base_dir "./runs/ckpts" \
            --dataset="sem_seg||refer_seg||vqa||reason_seg||grandf||refer_vos||mevis||vidstg||video_vqa||anet_gcg||video_gcg||mevis_gcg||vidstg_gcg||hcstvg_gcg" \
            --sample_rates_for_datasets="1,1,1,1,20,1,1,1,1,1,20,5,20,20,10" \
            --train_mask_decoder=False \
            --tune_mm_mlp_adapter=True \
            --use_sam_version='v2' \
            --precision='fp16' \
            --num_frames_for_sam=8 \
            --batch_size=1 \
            --grad_accumulation_steps=10 \
            --epochs=30 \
            --auto_resume

