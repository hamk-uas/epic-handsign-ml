# epic-handsign-ml
Machine learning to infer sign language letters from hand tracking data

<img alt="Preprocessing worklfow" src="preprocessing workflow.svg"/>

Notebooks:
- `video-timestamp-ocr.ipynb` - Optical character recognition (OCR) of spectator camera video timestamps
- `package-training-data.ipynb` - Preprocess and package training data
- `gesture-classification-demo.ipynb` - Training data augmentation and machine learning model training

Input data files:
- `annotation schema.yml` - Annotation schema for VideoAnnotator and `package-training-data.ipynb`
- `2022-03-18 17-07-41 annotation.json` - Manual annotation data from VideoAnnotator, needed by `package-training-data.ipynb`
- `2022-03-18 17-07-41 hand tracking data.csv` - Hand tracking data, needed by `package-training-data.ipynb`

Intermediate output data files:
- `2022-03-18 17-07-41 timestamps.csv` - Video timestamp OCR result from `video-timestamp-ocr.ipynb`, needed by `package-training-data.ipynb`

Output image files for visualization:
- `frame0.png` - Sample video frame from `video-timestamp-ocr.ipynb`
- `frame0_crop.png` - Sample cropped video timestamp from `video-timestamp-ocr.ipynb`
- `training data preprocessing result.svg` - Summary of training data preprocessing from `package-training-data.ipynb`
- `training data preprocessing result (edit).svg` - The same, with SVG errors fixed

Output data files:
- `2022-03-18 17-07-41 training data.csv` - Preprocessed training data from `package-training-data.ipynb`
