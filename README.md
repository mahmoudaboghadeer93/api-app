## Helm Package

1️⃣ package my Project

```shell
   helm package api-app
   mv api-app-0.1.0.tgz charts/
  
```

2️⃣ Push image to DockerHub

```shell
   cd charts
   helm repo index . --url https://mahmoudaboghadeer93.github.io/api-app/charts
   cd ..
```

3️⃣ Push chart to github

```shell
   git add .
   git commit -m "Add Helm chart"
   git push origin main  
```

🎉 We are done, now have our own [**chart**](https://artifacthub.io/packages/helm/api-app/api-app-chart). 🎉