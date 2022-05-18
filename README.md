# RealTimeObjectDetection

Create a conda env;
  conda create -n asldev python==3.6 -y
  
  
Install the packages required;
  pip install -r requirements.txt
  
  
for Inference and training you will need to run main.ipynb.


for collecting data;

  use your camera to collect images.
  
  use labelImg repo located in Tensorflow/ to label your dataset 
  
  to use labelimg install requirements.txt located in requirements/
  
  set ouptut and input directory & tick autosave.
  
  
for training;

  split dataset in train and test folders located in Tensorflow/workspace/images
  
  create a directory my_ssd_mobnet in Tensorflow/workspace/models
  
  copy Tensorflow/workspace/pre-trained-models/ssd_mobilenet_v2_fpnlite_320x320_coco17_tpu-8/pipeline.config to our   created directory my_ssd_mobnet
  
  
  In main.ipynb;
  
    create a label map respective to the number of labels in your dataset.
    
    change the number of classes respective to your dataset by changing the pipeline_config.model.ssd.num_classes in the notebook
    
    run Train the model cell and copy the output to the terminal and run it.
    
    
  
  
