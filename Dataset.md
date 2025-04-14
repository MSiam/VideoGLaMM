### **Datasets used for training VideoGLaMM**

- **LISA datasets**: [Link](https://mbzuaiac-my.sharepoint.com/:u:/g/personal/shehan_munasinghe_mbzuai_ac_ae/Ed6NO_HzOtxHuLUtwU5llQoBNTKW-hWsat_ADhMPBhdrVA?e=eVFlLu)
- **GranDf dataset**: [Link](https://mbzuaiac-my.sharepoint.com/:u:/g/personal/shehan_munasinghe_mbzuai_ac_ae/EX4whuRa1NdEihJGAIL1j0MBvF8xvx22tX9D3g3lNhW_VQ?e=Y23PDA)
- **Video datasets**:
  - **ActivityNet**: [Link](https://drive.google.com/file/d/1qW5bLQtOienpMjO7vkaghA3pCPXc1qj9/view?usp=sharing)
  - **ActivityNet Captions**: [Link](https://drive.google.com/file/d/13tlKsXTA7YLwN62h_OjxmNulWBjbweNF/view?usp=sharing)
  - **ActivityNet Entities**: [Link](https://drive.google.com/file/d/13uYeYjXNW9mvsLpuLcNCpp2Zle-HuaUS/view?usp=sharing)
  - **BURST**: [Link](https://drive.google.com/file/d/119syWknOhxX9HGedkerk9kQo6MHBBQVQ/view?usp=sharing)
  - **HC-STVG**: [Link](https://drive.google.com/file/d/1pzK3aP4bMfpUA1dzSXC9GCxypHgZA1aL/view?usp=sharing)
  - **MeViS**: [Link](https://drive.google.com/file/d/1uuE2IcD4UGpkFdD2MWrIlVVN48PVoXRT/view?usp=sharing)
  - **Processed**: [Link](https://drive.google.com/file/d/1Z16c1WgmoqsUa557ILIG2QBy0hit5Nhr/view?usp=sharing)
    - ActivityNet Entities
    - HC-STVG
    - Referring DAVIS
    - VideoInstruct100K
    - VidSTG
  - **Refer DAVIS**: [Link](https://drive.google.com/file/d/1B4uHyt3_KZIFs9bQobowkPg1y0tG0IuO/view?usp=sharing)
    - DAVIS 16
    - DAVIS 17
  - **Refer YouTube-VOS**: [Link](https://drive.google.com/file/d/1zApsra2fqGX8b3diSvhIfe7bBjZW9tJI/view?usp=sharing)
  - **VideoInstruct100K**: [Link](https://drive.google.com/file/d/1l6XKWbX40tGIG1K05iBW8q4QFfDA-2_1/view?usp=sharing)
  - **VidSTG**: [Link](https://drive.google.com/file/d/12INPWw_FAQcXkeIgGdm61vJ35tkJeGAF/view?usp=sharing)
  - **YTVIS**: [Link](https://mbzuaiac-my.sharepoint.com/:u:/g/personal/shehan_munasinghe_mbzuai_ac_ae/EQIEnJmu1yhIhjkwRD8fVcYBRHaQFI9CmZDOoLRkmCXOBw?e=cbDr28)

- **GCG Datasets**:
  - **ActivityNet Entities GCG**: [Link](https://mbzuaiac-my.sharepoint.com/:u:/g/personal/shehan_munasinghe_mbzuai_ac_ae/EaG0sNQ--y1CjVf7WeYdahEBy2l6LQOvo_shVZqY22YRHg?e=r9itQ5)
  - **Burst-YTVIS GCG**: [Link](https://mbzuaiac-my.sharepoint.com/:u:/g/personal/shehan_munasinghe_mbzuai_ac_ae/EThjSLl_aMhIka6S1KxiqEEBf9rUCKNbX9LVyg60rw6Urg?e=wyhMsC)
  - **Refer-YTVOS GCG**: [Link](https://mbzuaiac-my.sharepoint.com/:u:/g/personal/shehan_munasinghe_mbzuai_ac_ae/EYy0FJi1PCxBiyudE-z9M6UBu-Ceae-mpjQ8w7aQ7c6KAA?e=VKUcoP)
  - **VidSTG GCG**: [Link](https://mbzuaiac-my.sharepoint.com/:u:/g/personal/shehan_munasinghe_mbzuai_ac_ae/EQhWEdhvCX1OkSSYPcnX9KsBrlw1AeTSffUtiD8K7wsc8w?e=FIEqEA)
  - **HC-STVG GCG**: [Link](https://mbzuaiac-my.sharepoint.com/:u:/g/personal/shehan_munasinghe_mbzuai_ac_ae/EaVtsayKs9ZIg83K36F9YC8B-7HiPa-SW3AXDT3-28m_Zw?e=H3dWQK)
  - **MeViS GCG**: [Link](https://mbzuaiac-my.sharepoint.com/:u:/g/personal/shehan_munasinghe_mbzuai_ac_ae/EcMipuuIMx9AofwShTCzAB8BVtLiRDJoFjPDTNnY48gv8Q?e=6tTTBx)


### **File Structure**

Extract **LISA dataset** and **GranDf dataset** under `./dataset`:

    dataset/
    ├── ade20k
    ├── coco
    ├── cocostuff
    ├── grandf_dataset
    ├── llava_dataset
    ├── mapillary
    ├── other
    ├── reason_seg
    ├── refer_seg
    └── vlpart

Extract **other datasets** under `./video_dataset`:

    video_dataset/
    ├── activitynet
    ├── activitynet_captions
    ├── activitynet_entities
    ├── activitynet_entities_gcg
    ├── burst
    ├── hcstvg
    ├── hcstvg_gcg
    ├── mevis
    ├── mevis_gcg
    ├── processed
    ├── refer_davis
    ├── refer_youtube_vos
    ├── video_gcg
    ├── video_instruct_100k
    ├── vidstg
    ├── vidstg_gcg
    ├── ytvis
    └── ytvos_gcg

