all : RemotingConfiguration_GetRegisteredActivatedService_server.exe RemotingConfiguration_GetRegisteredActivatedService_client.exe RemotingConfiguration_GetRegisteredActivatedService_shared.dll

RemotingConfiguration_GetRegisteredActivatedService_shared.dll : RemotingConfiguration_GetRegisteredActivatedService_shared.vb
	vbc /debug+ /nologo /t:library RemotingConfiguration_GetRegisteredActivatedService_shared.vb

RemotingConfiguration_GetRegisteredActivatedService_server.exe : RemotingConfiguration_GetRegisteredActivatedService_server.vb RemotingConfiguration_GetRegisteredActivatedService_shared.dll
	vbc /debug+ /nologo /r:RemotingConfiguration_GetRegisteredActivatedService_shared.dll RemotingConfiguration_GetRegisteredActivatedService_server.vb

RemotingConfiguration_GetRegisteredActivatedService_client.exe : RemotingConfiguration_GetRegisteredActivatedService_client.vb RemotingConfiguration_GetRegisteredActivatedService_shared.dll
	vbc /debug+ /nologo /r:RemotingConfiguration_GetRegisteredActivatedService_shared.dll RemotingConfiguration_GetRegisteredActivatedService_client.vb

