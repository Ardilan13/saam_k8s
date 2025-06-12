Para correr el proyecto de saam usando kubernetes, sigue estos pasos:
1. **Instalar Docker**: Asegúrate de tener Docker instalado en tu máquina.
2. **Instalar Kubernetes**: Usando Minikube.
3. **Correr el clúster de Kubernetes**: Ejecuta `minikube start` para iniciar el clúster.
4. **Correr kubectl**: Asegúrate de que `kubectl` esté instalado y configurado para interactuar con tu clúster de Minikube y corre kubectl apply -f .
5. **Verificar el estado de los pods**: Usa `kubectl get pods` para verificar que todos los pods estén corriendo correctamente.
6. **Acceder a la aplicación**: Usa `minikube service saam-service` para acceder a la aplicación desde tu navegador.
7. **Verificar logs**: Si necesitas verificar los logs de un pod específico, usa `kubectl logs <nombre-del-pod>`.
8. **Detener Minikube**: Cuando hayas terminado, puedes detener Minikube con `minikube stop`.
9. **Eliminar Minikube**: Si deseas eliminar el clúster de Minikube, usa `minikube delete`.