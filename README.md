# Regresion Logistica

Aplicando la regresión logística para el mismo caso de los medicamentos pero con un enfoque diferente en esta ocasión, buscando determinar si el medicamento recomendado seria nacional o extrangero, comenzamos con el ingreso de los datos y su organización.
<br>![image](https://github.com/user-attachments/assets/76d9a99f-ae6f-4a9b-98a5-4a56ffe8b7be)

Nuevamente realizamos el preprocesamiento y esta vez re asignamos los valores del medicamento para que se ajuste al resultado deseado, 0 para nacional y 1 para extrangero.
<br>![image](https://github.com/user-attachments/assets/31c9d2a3-8b05-41d7-b5e5-7233a3c5df76)

Realizamos la separación de grupos de prueba y entrenamiento
<br>![image](https://github.com/user-attachments/assets/d8ffcfa2-0154-46ee-92bb-8342d420b40a)

A partir de este punto realizamos la evaluación de los modelos con los diferentes solucionadores: sag, newton-cg, liblinear, saga y lbfgs.
<br>![image](https://github.com/user-attachments/assets/45df1faf-23f2-4b99-99c9-fa6e0276741e)
<br>![image](https://github.com/user-attachments/assets/97ba2ace-9c22-4289-a998-07f0631a4d79)
<br>![image](https://github.com/user-attachments/assets/d606171a-782f-45ad-a8e4-a9bd333ebe3c)
<br>![image](https://github.com/user-attachments/assets/5a0337c8-725f-457b-aae2-76c0d7a5ca35)
<br>![image](https://github.com/user-attachments/assets/30ef376c-9ae4-4a12-a3e8-1c51198af810)

***Predicciones***

Después de correr este modelo con los diferentes solucionadores, obtenemos que los mejores para este caso son: newton-cg, liblinear y lbfgs dándonos los mismo resultados y colores, con 98% de precisión en cada uno.
<br>![image](https://github.com/user-attachments/assets/2686e3b6-a4da-4772-b656-979cc11f8ad1)

Podemos ver que con esta prueba rápida las predicciones son certeras.

Seguimos con la graficaciones de la curva ROC
<br>![image](https://github.com/user-attachments/assets/88cab96a-1c9b-4f0f-9482-3d9cae2f2aa2)
<br>![image](https://github.com/user-attachments/assets/da08deb8-f8e5-4384-83dc-3dcbc40fb600)

Mediante esta gráfica podemos ver que los resultados de las predicciones fueron completamente certeros al compararlos con los valores reales obteniendo la máxima área bajo la curva y comprobando que este modelo es confiable para este caso utilizando cualquiera de los solucionadores newton-cg, liblinear o lbfgs
