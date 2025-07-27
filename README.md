# AI Task: Traffic Scene Understanding

## 🎯 Objective
Build a pipeline that takes an image of a traffic scene and outputs:
- A JSON with object detections (cars, traffic lights, etc.)
- Detected license plates with OCR
- Scene description using BLIP-2

## 🧱 Pipeline Components
1. **YOLOv8** for object detection
2. **Custom YOLOv8 model** for license plates
3. **PaddleOCR** for text recognition
4. **BLIP-2 (HuggingFace)** for scene captioning

## ⚙️ Adjustable Parameters
- YOLO confidence threshold
- OCR confidence threshold
- VLLM temperature/top_p

## 🖼️ Sample Inputs & Outputs
Input Image:
![sample](test_images/sample.jpg)

Sample Output JSON:
```json
{
  "scene_description": "7 cars, 3 traffic lights",
  "license_plates": [
    {"text": "LU01J10", "confidence": 0.96}
  ]
}
```
## 🚀 How to Run
Colab
Open the notebook: Objects_Task.ipynb

Upload your image(s)

Run all cells
