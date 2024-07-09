# [The COCO-CF Dataset in ECCV Paper: Improving Vision and Language Concepts Understanding with Multimodal Counterfactual Samples]()

[//]: # (### Requirements)

[//]: # (- [PyTorch]&#40;https://pytorch.org/&#41; 1.9 or higher)

[//]: # (- [CLIP]&#40;https://github.com/openai/CLIP&#41; &#40;install with `pip install git+https://github.com/openai/CLIP.git`&#41;)

[//]: # (- [transformers]&#40;https://huggingface.co/docs/transformers/index&#41; &#40;install with `pip install transformers`&#41;)

[//]: # (- [diffusion]&#40;https://colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/stable_diffusion.ipynb&#41; for text-to-image generation &#40;install with `pip install scipy ftfy accelerate diffusers `&#41;)


#####  COCO-CF is the dataset which is automatically generated from MS-COCO by injecting concepts from off-the-shelf language models and diffusion models to reduce the bias of bag-of-objects.
### Illustration
- The counterfactual images and captions in COCO-CF dataset can be download in [BaiduYun Drive](https://pan.baidu.com/s/1natTvj0x0PKF8-dPzFTqOA?pwd=id93)
- The factual images and captions can be download in [COCO website](https://cocodataset.org/#home)
- The samples of COCO-CF are shown in Directory 'COCO-CF-Example'

##### The structure of the Directory "COCO-CF-Example"

```bash
-COCO-CF-Example
---images
    --COCO_train2014_000000001122.jpg
    --COCO_train2014_000000001122_2113.jpg
    .
    .
    .
    --COCO_train2014_000000001907_138726.jpg
---coco-cf.json
```
##### The structure of the file "coco-cf.json" in the directory
```bash
[
    {
        "factual": {
            "image": "COCO_train2014_000000001122.jpg",
            "caption": "a red and yellow trains engine pulling its cars and some tracks"
        },
        "counterfactual": {
            "image": "COCO_train2014_000000001122_2113.jpg",
            "caption": "a blue and yellow trains engine pulling its cars and some tracks"
        }
    }
]
```
