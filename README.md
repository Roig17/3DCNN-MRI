# 3DCNN-MRI-Binary-Classification

Español (Scroll down for English)

Aquí puedes encontrar el código Python para preprocesar, realizar data augmentation y clasificar, mediante redes convolucionales, imágenes de resoancia magnética entre sujetos sanos y pacientes. Todo el codigo esta comentado en castellano y en ingles.

El codigo de preDprocess utiliza el paquete nipype y es facilmente generalizable. Para mas informacion y tutoriales sobre nipype:
Documentacion y ejemplos: https://nipype.readthedocs.io/en/latest/#
Turtoriales: https://miykael.github.io/nipype-beginner-s-guide/

El codigo para la red neuronal convolucional en 3D esta implementado en Tensorflow/Keras y es facilmente generalizable. Puedes encontrar un tutorial
sobre una red neuronal similar aplicada a imagen medica en:
https://keras.io/examples/vision/3D_image_classification/

El codigo para realizar el data augmentation esta pensado para leer las imagenes, realzar data augmentation y histogram matching, y guardar las nuevas imagenes. TorchIO no esa pensado
para ese proceso (realiza el data augmentation durante el entrenamiento para ahorrar memoria). Por esto el codigo es poco generalizable e incluso confuso. Por suerte torchIO tiene grandes tutoriales:
Documentacion TorchIO:  https://torchio.readthedocs.io/
Tutoriales torchIO:https://github.com/fepegar/torchio/blob/master/notebooks/README.md

Si vas a usar TorcchIO para realizar el data augmentation te recomiendo que utilices Pytorch en lugar de Keras para implementar el modelo, ya que torchio
esta pensado para ello.

English

Here you can find the Python code for preprocessing, data augment and classify magnetic resonance images using convolutional neural networks. All the code
is comented in both spanish and english

The code for the preprocessing step is mainly done using nipype library and it is easy to generalize. For more information an tutorials on nipype:
Docs and examples: https://nipype.readthedocs.io/en/latest/#
Tutorials: https://miykael.github.io/nipype-beginner-s-guide/

The code for the 3D convolutional neural network is implemented in Tensorflow/Keras and it is easy to generalize. For a similar net tutorial on medical image:
https://keras.io/examples/vision/3D_image_classification/

Data augmetation is implemented so images are read, data augmetation and histogram matching is performed, and all new iamges are saved into disk. TorchIO is not ment to use it that way, (it is ment to perform data augmentation during training in order to avoid memory issues). That is the reason why the code can be a little difficult to generalize. You can find everything about torchIO in:
Documentation: https://torchio.readthedocs.io/
Tutorials: https://github.com/fepegar/torchio/blob/master/notebooks/README.md

If you are going to use TorchIO for data augmentation I strongly recommend you to use Pytorch instead of Keras for implementing the neural network, as TorchIO
is implemented for it.

