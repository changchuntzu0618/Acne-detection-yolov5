# Acne-detection-yolov5-
This model "best.pt" is an acne detection model trained with yolov5 and publicly avaliable dataset "ACNE-04".
Please refer to yolov5 page for the code:  https://github.com/ultralytics/yolov5
How to use:
    1. Download code from  https://github.com/ultralytics/yolov5
	  2. required packages are in: requirements.txt. U may use following command in terminal to install all required packages
		>>pip install -r yolov5/requirements.txt
    detect.py:use this one for inference/implementation
	#run following command in terminal
	>>python detect.py --source location of dataset --weights ...\best.pt --conf 0.25 --name ...
	##--source flag: 
		defines the source of our detector, which can be: 
		1. A single image 2. A folder of images
		3. Video 4. Webcam(ex. --source 0)
	##--weights flag:
		defines the path of the model which we want to run our detector with. 
	##--conf flag: 
		the thresholding objectness confidence.
	##--name flag:
		defines where the detections are stored. if we set this flag to yolo_acne_det; therefore, the detections would be stored in runs/detect/yolo_acne_det/

The model achieves a satisfactory performance with mAP@.5 value of 38.5.
