# cache

This folder is the cache directory for Hugging Face (HF).

When using online mode, downloaded models will be cached in this folder.

For [offline mode](https://huggingface.co/docs/transformers/main/installation#offline-mode) use, please download the models in advance and specify the model directory.


## Directory structures

**There are currently two directory structures:**
- The Huggingface CLI cache structure

### Huggingface CLI cache structure

use this command `tree -a ./cache/huggingface/hub`

```
./cache/huggingface/hub
├── models--OmniSVG--OmniSVG
│   ├── blobs
│   │   ├── 41678afb8394c79a86381e53588ce4f18b4bb9dd
│   │   ├── 64be7bb0bbd8c1d7df8c153703c671db338b0e426c872554770d21e9db9cf90c
│   │   ├── a6344aac8c09253b3b630fb776ae94478aa0275b
│   │   ├── c5ee2f889dd3c8ce604e8b11ed6bac42be56044d
│   │   └── f466c7edd301d2e639b667da2714f006fd83b1a0
│   ├── refs
│   │   └── main
│   └── snapshots
│       └── 40138c74a343eae6c0d1149e0dbe95b163db0665
│           ├── config.json -> ../../blobs/41678afb8394c79a86381e53588ce4f18b4bb9dd
│           ├── config.yaml -> ../../blobs/c5ee2f889dd3c8ce604e8b11ed6bac42be56044d
│           ├── pytorch_model.bin -> ../../blobs/64be7bb0bbd8c1d7df8c153703c671db338b0e426c872554770d21e9db9cf90c
│           └── README.md -> ../../blobs/f466c7edd301d2e639b667da2714f006fd83b1a0
├── models--OmniSVG--OmniSVG1.1_4B
│   ├── blobs
│   │   ├── 2a6fc63a96e64067c88eddab3a6ba8ad3577b468
│   │   ├── 39f36759fc677b329e01b5b34cf7c96a5b1922b659d65d80d565e3d782f5a6c4
│   │   └── a6344aac8c09253b3b630fb776ae94478aa0275b
│   ├── refs
│   │   └── main
│   └── snapshots
│       └── e4d03a89aaa28468520b45dc2541098102264d4e
│           ├── pytorch_model.bin -> ../../blobs/39f36759fc677b329e01b5b34cf7c96a5b1922b659d65d80d565e3d782f5a6c4
│           └── README.md -> ../../blobs/2a6fc63a96e64067c88eddab3a6ba8ad3577b468
├── models--OmniSVG--OmniSVG1.1_8B
│   ├── blobs
│   │   ├── 08c9ef282c713d13e36527221f54031f344f9034349000a49d05e0f660a5b5a8
│   │   ├── 656bfc53ef22c757796e639a3fdcfed9d031cad7
│   │   └── a6344aac8c09253b3b630fb776ae94478aa0275b
│   ├── refs
│   │   └── main
│   └── snapshots
│       └── ce0d49d5b92b27590e2d7747a31c17d70e914c8b
│           ├── pytorch_model.bin -> ../../blobs/08c9ef282c713d13e36527221f54031f344f9034349000a49d05e0f660a5b5a8
│           └── README.md -> ../../blobs/656bfc53ef22c757796e639a3fdcfed9d031cad7
├── models--Qwen--Qwen2.5-VL-3B-Instruct
│   ├── blobs
│   │   ├── 0ae1866f05ab0153ad293bdc92bb1b842c4d95b1
│   │   ├── 1dfafa23e24b68b694722c6211e7da36730e9917
│   │   ├── 20024bfe7c83998e9aeaf98a0cd6a2ce6306c2f0
│   │   ├── 365531ff8752420e89dee707b79d021fb2d6e25abafe486f080555a4fe6972e4
│   │   ├── 41a8895c164b4d32bae6b302f4603fcbc1797f32dafa45c7e9bcda23c6755df8
│   │   ├── 443909a61d429dff23010e5bddd28ff530edda00
│   │   ├── 4783fe10ac3adce15ac8f358ef5462739852c569
│   │   ├── 732bd68bc5427d1fb6c06a59b3bf2456b2155d24
│   │   ├── 7a3ec4f48662e38593f8cab48fe12a4f28003aba
│   │   ├── 7f3b746825e5eef53ed8ed57a91df9e86ee62c0a
│   │   ├── 87f48cf86671d627b4dd4b8e5189b8e32ae11dd8
│   │   ├── 91684ea3dc135a7d815e2c932054ce88c1aab41f
│   │   ├── a6344aac8c09253b3b630fb776ae94478aa0275b
│   │   └── d09bc2825f7d1dc394ee6766e2e95bcc59f47196
│   ├── refs
│   │   └── main
│   └── snapshots
│       └── 66285546d2b821cf421d4f5eb2576359d3770cd3
│           ├── chat_template.json -> ../../blobs/732bd68bc5427d1fb6c06a59b3bf2456b2155d24
│           ├── config.json -> ../../blobs/0ae1866f05ab0153ad293bdc92bb1b842c4d95b1
│           ├── generation_config.json -> ../../blobs/1dfafa23e24b68b694722c6211e7da36730e9917
│           ├── LICENSE -> ../../blobs/87f48cf86671d627b4dd4b8e5189b8e32ae11dd8
│           ├── merges.txt -> ../../blobs/20024bfe7c83998e9aeaf98a0cd6a2ce6306c2f0
│           ├── model-00001-of-00002.safetensors -> ../../blobs/41a8895c164b4d32bae6b302f4603fcbc1797f32dafa45c7e9bcda23c6755df8
│           ├── model-00002-of-00002.safetensors -> ../../blobs/365531ff8752420e89dee707b79d021fb2d6e25abafe486f080555a4fe6972e4
│           ├── model.safetensors.index.json -> ../../blobs/7a3ec4f48662e38593f8cab48fe12a4f28003aba
│           ├── preprocessor_config.json -> ../../blobs/7f3b746825e5eef53ed8ed57a91df9e86ee62c0a
│           ├── README.md -> ../../blobs/d09bc2825f7d1dc394ee6766e2e95bcc59f47196
│           ├── tokenizer_config.json -> ../../blobs/91684ea3dc135a7d815e2c932054ce88c1aab41f
│           ├── tokenizer.json -> ../../blobs/443909a61d429dff23010e5bddd28ff530edda00
│           └── vocab.json -> ../../blobs/4783fe10ac3adce15ac8f358ef5462739852c569
└── models--Qwen--Qwen2.5-VL-7B-Instruct
    ├── blobs
    │   ├── 0c859795ad3a627a9b95bcb762e059d5b768a4a36fdd4affeff269d93fdecc67
    │   ├── 1088c9865dbf2e8152485664bb07495e89a14efb
    │   ├── 111223d173e00bbee81cba1216fad28668df3476706b7fd26f4d5b50f8b3a507
    │   ├── 20024bfe7c83998e9aeaf98a0cd6a2ce6306c2f0
    │   ├── 443909a61d429dff23010e5bddd28ff530edda00
    │   ├── 4783fe10ac3adce15ac8f358ef5462739852c569
    │   ├── 58ee12a9fb3d8708a1e41e49cb9aa5ac5017b6a6
    │   ├── 5f169031e3f61faa8262272000c36d54bdc9b926
    │   ├── 732bd68bc5427d1fb6c06a59b3bf2456b2155d24
    │   ├── 7f3b746825e5eef53ed8ed57a91df9e86ee62c0a
    │   ├── 91684ea3dc135a7d815e2c932054ce88c1aab41f
    │   ├── a6344aac8c09253b3b630fb776ae94478aa0275b
    │   ├── a9a300a43b4724eee2abe7c18ceb26768d0ab011eb0cad19d9bfd2476a24d024
    │   ├── e97b877e47fde53a6c6e77aafb36e58e91ee9d95c4a3eeac6f1b5c0e6a1c986e
    │   ├── ef47f634fa57d46ee134edcc09f34085a47da1e16c12a2abe0d67118be6d72ed
    │   └── f0c9e9b8e043f5de0ac99fd8b2ea75515d811e7b
    ├── refs
    │   └── main
    └── snapshots
        └── cc594898137f460bfe9f0759e9844b3ce807cfb5
            ├── chat_template.json -> ../../blobs/732bd68bc5427d1fb6c06a59b3bf2456b2155d24
            ├── config.json -> ../../blobs/58ee12a9fb3d8708a1e41e49cb9aa5ac5017b6a6
            ├── generation_config.json -> ../../blobs/1088c9865dbf2e8152485664bb07495e89a14efb
            ├── merges.txt -> ../../blobs/20024bfe7c83998e9aeaf98a0cd6a2ce6306c2f0
            ├── model-00001-of-00005.safetensors -> ../../blobs/e97b877e47fde53a6c6e77aafb36e58e91ee9d95c4a3eeac6f1b5c0e6a1c986e
            ├── model-00002-of-00005.safetensors -> ../../blobs/a9a300a43b4724eee2abe7c18ceb26768d0ab011eb0cad19d9bfd2476a24d024
            ├── model-00003-of-00005.safetensors -> ../../blobs/111223d173e00bbee81cba1216fad28668df3476706b7fd26f4d5b50f8b3a507
            ├── model-00004-of-00005.safetensors -> ../../blobs/ef47f634fa57d46ee134edcc09f34085a47da1e16c12a2abe0d67118be6d72ed
            ├── model-00005-of-00005.safetensors -> ../../blobs/0c859795ad3a627a9b95bcb762e059d5b768a4a36fdd4affeff269d93fdecc67
            ├── model.safetensors.index.json -> ../../blobs/f0c9e9b8e043f5de0ac99fd8b2ea75515d811e7b
            ├── preprocessor_config.json -> ../../blobs/7f3b746825e5eef53ed8ed57a91df9e86ee62c0a
            ├── README.md -> ../../blobs/5f169031e3f61faa8262272000c36d54bdc9b926
            ├── tokenizer_config.json -> ../../blobs/91684ea3dc135a7d815e2c932054ce88c1aab41f
            ├── tokenizer.json -> ../../blobs/443909a61d429dff23010e5bddd28ff530edda00
            └── vocab.json -> ../../blobs/4783fe10ac3adce15ac8f358ef5462739852c569

26 directories, 82 files
```

## Pre-download for offline mode

Running in online mode will automatically download the model.

### use huggingface-cli

install cli

```bash
pip install -U "huggingface_hub[cli]"
```

download model

```bash
hf download OmniSVG/OmniSVG1.1_8B --cache-dir ./cache/huggingface/hub
hf download Qwen/Qwen2.5-VL-7B-Instruct --cache-dir ./cache/huggingface/hub
hf download OmniSVG/OmniSVG1.1_4B --cache-dir ./cache/huggingface/hub
hf download Qwen/Qwen2.5-VL-3B-Instruct --cache-dir ./cache/huggingface/hub
hf download OmniSVG/OmniSVG --cache-dir ./cache/huggingface/hub
```
