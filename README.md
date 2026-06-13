# Detecção de Fadiga no Trânsito

---
#### Projeto da Disciplina PET1706 - TÓPICOS ESPECIAIS EM ENGENHARIA DE SOFTWARE (Redes Neurais Artificiais) - 2026.1 
###### Professora: [Rosana Rego](https://github.com/roscibely)
<div>
  <img src="https://raw.githubusercontent.com/roscibely/algorithms-and-data-structure/main/root/ufersa.jpg" width="700" height="250">
</div>
<i> <a href="https://engsoftwarepaudosferros.ufersa.edu.br/apresentacao/"> Curso Bacharel em Engenharia de Software  </a> - UFERSA - Campus Pau dos Ferros </a></i>

---

O projeto tem o objetivo de identificar fadiga/sonolência em motoristas através de classificação de imagens utilizando Redes Neurais Convolucionais. O sistema detecta sinais visuais como olhos fechados e bocejos.

## Funcionalidades Principais

- **Detecção de Fadiga**: Classifica imagens de olhos em duas categorias: fadiga (olhos fechados ou bocejando) e alerta (olhos abertos)
- **Modelos Implementados**: CNN personalizada e MobileNet para otimização de performance
- **Explicabilidade (XAI)**: Utiliza SHAP para explicabilidade das predições

## Requisitos da aplicação

- Python 3.8+
- Conexão com internet (para download do dataset na primeira execução)
- Bibliotecas Python: TensorFlow, Keras, NumPy, OpenCV, scikit-learn (detalhes no arquivo `requirements.txt`)
- (Opcional) GPU NVIDIA com CUDA para aceleração do treinamento

## Instalação

1. Clone o repositório do GitHub:

```bash
git clone https://github.com/ClassNeuralNetwork/classification-fatigue-detection.git
```

2. Navegue até o diretório do projeto:

```bash
cd classification-fatigue-detection
```

3. Instale as dependências usando pip:

```bash
python -m pip install -r requirements.txt
```

## Uso

O projeto oferece dois notebooks com diferentes abordagens:

### 1. **CNN Personalizada** (`Deteccao_Sonolencia_CNN.ipynb`)
Implementação de uma Rede Neural Convolucional com arquitetura ConvNeXtLarge para detecção de fadiga com alta precisão.

### 2. **MobileNet** (`Deteccao_Sonolencia_MobileNet.ipynb`)
Utiliza transfer learning com MobileNet, otimizado para performance e menor uso de recursos computacionais.

Para executar qualquer um dos notebooks:

```bash
jupyter notebook Deteccao_Sonolencia_CNN.ipynb
# ou
jupyter notebook Deteccao_Sonolencia_MobileNet.ipynb
```

## Dataset

O projeto utiliza o **Yawn Eye Dataset (YED)**, que contém:
- **Imagens de olhos abertos** (Alerta)
- **Imagens de olhos fechados** (Fadiga)
- **Imagens de bocejos** (Fadiga)
- **Imagens de olhos em diferentes ângulos** (Variações)

Dataset disponível em: [Kaggle - Yawn Eye Dataset New](https://www.kaggle.com/datasets/serenaraju/yawn-eye-dataset-new)

## Modelos Treinados

Os modelos pré-treinados estão disponíveis no diretório raiz:
- `modelo_cnn_YE.h5` - Modelo CNN treinado
- `model_sonolencia.keras` - Modelo em formato Keras

## Contribuição

Contribuições são bem-vindas! Se você quiser contribuir para este projeto, por favor, abra uma issue para discutir as mudanças propostas ou envie um pull request.

## Licença

Este projeto está licenciado sob a [Licença MIT](https://opensource.org/licenses/MIT). Consulte o arquivo `LICENSE` para obter mais detalhes.

## Equipe
<table align="center">
  <tr>    
    <td align="center">
      <a href="https://github.com/angellusj">
        <img src="https://avatars.githubusercontent.com/u/123104907" 
        width="120px;" alt="Foto de Ângela M. A. Aquino no GitHub"/><br>
        <sub>
          <b>Ângela M. A. Souza</b>
         </sub>
      </a>
    <td align="center">
      <a href="https://github.com/Malicef">
        <img src="https://avatars.githubusercontent.com/u/123081912" 
        width="120px;" alt="Foto de Maria A. F. Teixeira no GitHub"/><br>
        <sub>
          <b>Maria A. F. Teixeira</b>
         </sub>
      </a>
    </td>
  </tr>
</table>
