# Flask-
python Flask安装
一、安装Virtualenv
pip install virtualenv
创建虚拟环境的目录，在任意目录中打开cmd，输入：virtualenv p3vir
启动虚拟环境：
p3vir\scripts\activate

二、安装flask
pip install Flask

三、使用PyCharm创建简单的Flask Web应用
ctrl+Alt+S 打开 Settings 面板，设置Projcet Interpreter ，选择虚拟环境的目录。
如果找不到创建的虚拟环境，可以在右边设置按钮中添加一个新的python interpreter， 
add local选择创建的虚拟环境venv中的python解释器（如D:\venv\Scripts\python.exe）就可以了

四、运行测试案例
from flask import Flask  
app = Flask(__name__)  
 
@app.route("/")  
def hello():  
    return "Hello World!"  
  
if __name__ == "__main__":  
    app.run() 

在IE中输入：http://127.0.0.1:5000/
