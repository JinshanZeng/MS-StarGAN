# MS-StarGAN
# Dependencies

Python 3.6+
TensorFlow 1.3+ (optional for tensorboard)

# datasets

Handwritten data download address：http://www.nlpr.ia.ac.cn/databases/handwriting/Download.html
Randomly extract an image of each font as our data set, and denoise、 resize as 128*128 、 strengthen pixels.

Standard datasets generate standard fonts from .ttf files of multiple fonts，and then resize them.

# Training networks

To train MS-StarGAN , run the training script below.  
If you change the selected_attrs argument, you should also change the c_dim argument accordingly.

# Train MS-StarGAN
python main.py

# test MS-StarGAN
change the code : parser.add_argument('--mode', type=str, default='test', choices=['train', 'test']) ，
and select your trained model ：parser.add_argument('--model_save_dir', type=str, default='')
