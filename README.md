helmchart for Devops_project_1 https://github.com/Brylov/Devops_Project_1


helm install portfolio-backend ./backend
helm install portfolio-frontend ./frontend --set frontend.API_URL="$(minikube service backend --url)/api"