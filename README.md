## REDE

-  ClusterIP resumidamente é habilitado apenas para a conexão interna, não têm acesso de fora.
-  NodePort é habilitado para o acesso de fora, se quiser subir e proxy na porta, fazer um port-forward.


## CONFIGMAP
- Para ter conexão local entre os clusters você deve, apontar dessa forma, por ex: conexão HTTP:

```
http://{NOME_DO_SERVICO}.{NAMESPACE}.svc.cluster.local:8081/api/dev
```
### ficaria:
```
http://storage-api-svc.storage-ns.svc.cluster.local:8081/api/dev
```