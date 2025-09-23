Bottle Detection Pipeline

This project is a cloud-native, frame-level object detection system designed to identify and track bottles in video footage—built for precision, scalability, and transparency. It leverages YOLOv5 for real-time detection, AWS Lambda for distributed processing, and S3 for structured result storage.

Features:

Frame-by-frame detection using YOLOv5 with tracker IDs and confidence scores

Cloud-native architecture powered by AWS Lambda and S3

Structured JSON output per frame, with automatic merging into a session-level summary

Confidence-based image selection to surface the best visual examples per bottle

Frontend integration for displaying detection summaries and curated thumbnails

Robust pipeline design with reproducible IDs, traceable results, and scalable processing

Motivation:

This project was born from the need to detect bottles in varied orientations and environments—especially in real-world footage where bottles may be lying flat, partially occluded, or distant. It aims to improve detection accuracy through custom training, smart post-processing, and thoughtful UI integration.

Technologies:

YOLOv5 for object detection

AWS Lambda for serverless frame processing

Amazon S3 for result storage and image hosting

JavaScript for frontend logic and dynamic image selection

Python for backend orchestration and merging logic

Future Plans:

Fine-tune YOLOv5 with custom bottle datasets (including flat and distant poses)

Add experiment tracking and confidence heatmaps

Integrate GPS or sensor overlays for spatial context

Expand to detect other recyclable materials