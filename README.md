images文件夹下应该同时包含.jpg与.json文件，且文件名一一对应<br>
labels.txt中需要修改自定义的类别，且必须符合如下要求：<br>
__ignore__<br>
__background__<br>
类别0<br>
类别1<br>
......<br>
类别n<br>
卡在当前目录下执行指令：<br>
python labelme2coco.py --input_dir images --output_dir coco --labels labels.txt<br>
执行完成后会自动创建名称为coco的文件夹，且自动划分训练集和测试集，coco文件夹不需要手动创建
