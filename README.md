# DSC180A-Quarter1-Integration

## Instructions for accessing AWS in local machine

1. Open terminal <br>
2. move to the repo directory: <br>
```cd DSC180A-Quarter1-Integration```<br>

3. Follow the command below to get access to AWS server <br>
``` ssh -i med1.pem ubuntu@54.186.34.136 ```

4. Follow the command below to get connected to Jupyter notebook<br>
``` sudo snap install jupyter ``` <br>
``` jupyter notebook --port=<4-digit-number> ```<br> 
Avoid using 8888 and try using other ports.<br>

5. Open up a new terminal <br>
``` ssh -i med1.pem ubuntu@54.186.34.136 -L <4-digit-number>:localhost:<4-digit-number> ```<br>
Avoid using 8888 and try using other ports.
