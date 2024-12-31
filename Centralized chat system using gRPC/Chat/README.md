1. For Python, to set up the plugin required for gRPC code generation, run 2 commands
    python3 -m pip install grpcio
    python3 -m pip install grpcio-tools

2. After cloning projectp, run the following command to install all the requirementsr:
    pip3 install -r requirements.txt

3. To generate the code from the proto schema in Python, run the following command:
    python3 -m grpc_tools.protoc -Iprotos --python_out=. --grpc_python_out=. protos/chatservice.proto

4. Run the server:
    python3 chatservice_server.py

5. Open 2 or more terminals to run the clients, execute the following command:
    python3 chatservice_client.py 

