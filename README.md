# bikerentalatividade
Atividade pra DIO sobre modelo de Machine Learning, usando dados de aluguel de bicicleta

1. Fiz o download do arquivo compactado "bike-data" através do link providenciado
2. Entrei no Azure Machine Learning Studio -> Automated ML
3. Criei uma nova tarefa, preenchendo os campos de acordo com as instruções na documentação
4. Fiz upload da pasta que extraí do arquivo compactado "bike-data"
5. Defini a tarefa como Regressão, com máximo de nós, avaliações e avaliações simultâneas em 3, e limitando a pontuação da métrica em 0,085
6. Após definir os outros dados como instruído, iniciei a tarefa, processo que levou um pouco menos de 10min
7. Após a computação terminar, selecionei o melhor modelo recomendado, e realizei um Deploy do modelo utilizando a opção Real-time Endpoint
8. Usei a máquina virtual Standard_E2s_v3, com Instance Count em 3, processo levou por volta de 10min
9. Terminado o Deploy, entrei na aba Endpoints, no Endpoint que acabou de ser criado, e então na aba Test
10. Substitui o código JSON que já estava presente pelo que foi recomendado
11. Realizei o Teste
12. Obtive o resultado 353.4709213849849 .
