# Covid19ctScans

## AI Backend System

For now, deployed under http://ec2-54-175-84-83.compute-1.amazonaws.com:5000/
To deploy in AWS:
- provision an ML EC2 instance using the following image: `Deep Learning AMI (Amazon Linux 2) Version 38.0`
- clone the git repo: `git clone https://github.com/PatienceMbuhNgong/Covid19ctScans.git`
- `cd Covid19ctScans`
- Install all required python modules: `pip3 install -r requirements.txt`
- Somehow this module was missed: `pip3 install opencv-python`
- Start the process:
```
export FLASK_APP=app.py
flask run --without-threads --host=0.0.0.0 &
disown
```

