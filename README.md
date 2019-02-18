# mnist-cnn


   A base MNIST é formada por dígitos entre 0 e 9 escritos a mão. É uma base composta por 60 mil imagens de treinamento e 10 mil imagens de teste, cada uma contendo o tamanho de 28x28 pixels. Foram criadas variáveis para as imagens da base de dados. As variáveis, x_train e y_train armazenam as imagens de treinamento e as variáveis de teste são armazenadas pelas variáveis x_test e y_test. 

  Os valores do filtro mudam a cada iteração de treinamento, com o objetivo de melhorar a identificação de quais regiões contém atributos significativos (da mesma forma que os pesos em um perceptron de uma rede neural são atualizados no treinamento). Mas como essa série de multiplicações nos ajuda a detectar os atributos de uma imagem? Conforme o filtro aprende a detectar um atributo (através do processo de aprendizado), seus valores se ajustam de forma que o resultado da convolução seja um valor que indique que o determinado atributo foi encontrado. É o mesmo mecanismo utilizado na detecção de spam/não spam explicada anteriormente, só que agora sendo aplicado a uma imagem.
Após os dados estarem prontos para serem alimentados ao modelo, precisamos definir a arquitetura do modelo e compilá-lo com a função otimizadora necessária, a função de perda e as métricas de desempenho. A arquitetura aqui seguida é de 2 camadas de convolução seguidas por camada de agrupamento, uma camada totalmente conectada e camada respectivamente. Vários filtros são usados em cada camada de convolução, para diferentes tipos de extração de recursos. Uma explicação intuitiva pode ser se o primeiro filtro ajuda a detectar as linhas retas na imagem, o segundo filtro ajudará na detecção de círculos e assim por diante. Depois que a arquitetura do modelo é definida e compilada, o modelo precisa ser treinado com dados de treinamento para poder reconhecer os dígitos manuscritos. Por isso, vamos encaixar o modelo com as variáveis x_train e y_train.
    
  



