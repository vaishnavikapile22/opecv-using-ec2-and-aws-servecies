# First need create instance 

#here i am using amzon linux os 

* IAM role is required and that attach to ec2-instance

* IAM users required for acess key

#connect to ssh

# follow thse cammond

sudo yum install python3

sudo yum install python3-pip

pip3 install opencv-python numpy boto3 termcolor matplotlib

mkdir myproject

# xml file for detect face and eye
 wget https://github.com/opencv/opencv/raw/master/data/haarcascades/haarcascade_frontalface_default.xml
 wget https://github.com/opencv/opencv/raw/master/data/haarcascades/haarcascade_eye.xml
 
mkdir opencv 

pip install awscli 

aws configure
Acess_key
Sceret key

thse is soln for error occur when file not run 
   
sudo apt-get install xvfb

sudo yum install xorg-x11-server-Xvfb

# Change ownership to ec2-user for the 'photo' directory and its contents

sudo chown -R ec2-user:ec2-user /home/ec2-user/opencv/photo/

# local to ec2

scp -i MUMBAI_KEY.pem srk.png ec2-user@35.154.28.254:/home/ec2-user/opencv/photo/

#ec2 to local

scp -i MUMBAI_KEY.pem ec2-user@3.109.133.244:/path/to/source/on/ec2/girl.png C:\Users\Admin\PycharmProjects\OPENCV


# RUN FILE

python detection.py -t photo/group.webp


Ec2 instance don't have direct permission for acess image so for that first we save image in form of.png file for image and .avi for vedio and then thse file transfer on local terminal i am using pycham and we easily see image



# OUPUT

THESE IS A JACKMA IMAGE

![result_with_eyes](https://github.com/vaishnavikapile22/opecv-using-ec2-and-aws-servecies/assets/149785862/1dd3816e-4038-4db5-a4d1-5ecd87cd7a75)
            

THESE IS A GROUP PHOTO

![result_with_eyes](https://github.com/vaishnavikapile22/opecv-using-ec2-and-aws-servecies/assets/149785862/980cb6a1-919d-4111-af8d-be07f5de7d79)
![Screenshot (33)](https://github.com/vaishnavikapile22/opecv-using-ec2-and-aws-servecies/assets/149785862/03dfc004-55f6-404d-8ac3-97ff24b8459a)
![Screenshot (34)](https://github.com/vaishnavikapile22/opecv-using-ec2-and-aws-servecies/assets/149785862/d9685dec-646f-4803-b567-1ad6e6452f6d)

THESE IS FOR VEDIO 

![output_vedio](https://github.com/vaishnavikapile22/opecv-using-ec2-and-aws-servecies/assets/149785862/246e15b2-9612-45c8-b502-67add9d2746f)
                 
