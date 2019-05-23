# face-recognition-opencv

dlib, face_recognition ve imutils kütüphaneleri gerekiyor.

Yüz öğretmek için dataset içindeki klasöre fotoğraflar atılıyor. 

Öğretmek için:

```shell
python encode_faces.py --dataset dataset --encodings encodings.pickle
```

Fotoğraftan tanımak için: 

```shell
python recognize_faces_image.py --encodings encodings.pickle --image examples/example_04.png
```

Videodan tanımak için: 

```shell
python recognize_faces_video_file.py --encodings encodings.pickle \
--input videos/lunch_scene.mp4 --output output/lunch_scene_output.avi \
--display 0
```
  
Kameradan tanımak için: 
  
```shell
python recognize_faces_video.py --encodings encodings.pickle \
--output output/webcam_face_recognition_output.avi --display 1
```
