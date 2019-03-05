# package
Package      Version  
certifi      2018.8.24  
grpcio       1.19.0  
grpcio-tools 1.19.0  
pip          10.0.1  
protobuf     3.7.0  
setuptools   40.2.0  
six          1.12.0  
wheel        0.31.1  
You are using pip version 10.0.1, however version 19.0.3 is available.  
You should consider upgrading via the 'pip install --upgrade pip' command.  
  
# cmd  
#1.install gRPC  
python -m pip install grpcio  
#2.install gRPC tools, including protoc built-in.  
python -m pip install grpcio-tools  
#3.build proto  
python -m grpc_tools.protoc -I./ --python_out=. --grpc_python_out=. ./hello.proto  
#4.run server  
python greeter_server.py  
#5.run client, please open another terminal to run this  
python greeter_client.py  
# output  
Greeter client received: Hello, goodspeed!  
