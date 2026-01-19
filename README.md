# 📏 Aplicativo de AR para Medição de Espaços - Projeto de Computação Gráfica

**Disciplina:** Computação Gráfica  
**Curso:** Engenharia da Computação  
**Instituição:** Universidade Federal do Maranhão (UFMA)  
**Semestre:** 2025.1  

---

## **Autores**

| Nome | Matrícula |
|------|-----------|
| DAVI OLIVEIRA CORTES | 20250013748 |
| LUCAS EMANOEL AMARAL GOMES | 20250071250 |

---

## **Descrição do Projeto**

Este projeto consiste em um aplicativo de **Realidade Aumentada (AR)** para medição de distâncias e áreas em ambientes reais, utilizando a câmera do dispositivo móvel. A aplicação foi desenvolvida como trabalho prático da disciplina de Computação Gráfica, com o objetivo de integrar conceitos de gráficos 3D, tracking de superfícies e interação em tempo real.

**Funcionalidades principais:**
- Medição de distância entre dois pontos no espaço real
- Detecção de planos horizontais e verticais
- Interface intuitiva com feedback visual
- Possibilidade de medições consecutivas

---

## **Tecnologias e Bibliotecas**

- **Unity** (2021.3 ou superior)
- **ARFoundation** (para abstração multiplataforma)
- **ARKit** (para dispositivos iOS)
- **ARCore** (para dispositivos Android)
- **C#** (linguagem de programação)

---

## **Passo a Passo para Executar no Unity**

### **Pré-requisitos**
1. Unity Hub instalado
2. Unity 2021.3 LTS ou superior
3. ARFoundation, ARCore XR Plugin e ARKit XR Plugin instalados via Package Manager

### **Configuração do Projeto no Unity**

1. **Clone o repositório**
   ```bash
   git clone [URL_DO_REPOSITORIO]
   ```

2. **Abra o projeto no Unity**
   - Inicie o Unity Hub
   - Clique em "Add" e selecione a pasta do projeto
   - Selecione a versão correta do Unity (2021.3+)

3. **Verifique os pacotes necessários**
   - Vá para `Window > Package Manager`
   - Certifique-se de que estão instalados:
     - ARFoundation (4.2.3+)
     - ARCore XR Plugin (4.2.3+)
     - ARKit XR Plugin (4.2.3+)

4. **Configure as Build Settings**
   - `File > Build Settings`
   - Selecione a plataforma desejada (Android ou iOS)
   - Clique em "Switch Platform"

5. **Configurações específicas para Android**
   - `Edit > Project Settings > Player`
   - Na aba "Other Settings":
     - **Minimum API Level**: Android 7.0 (API Level 24) ou superior
     - **Target API Level**: Mais recente instalado
     - Marque as opções:
       - **Multithreaded Rendering**
       - **Requires ARCore** (em XR Settings)

---

## **Build para Android**

### **Pré-requisitos para Android**
- JDK 11 ou superior instalado
- Android SDK instalado
- Device com ARCore suportado

### **Passos para Build**

1. **Configure o Player Settings**
   ```plaintext
   Edit > Project Settings > Player
   ```
   - Company Name: UFMA
   - Product Name: AR Measuring Tape
   - Version: 1.0

2. **Gere o Build**
   - `File > Build Settings`
   - Clique em "Add Open Scenes" para incluir a cena principal
   - Selecione "Android" como plataforma
   - Clique em "Build"
   - Escolha o local para salvar o arquivo `.apk`

3. **Instale no dispositivo**
   - Transfira o arquivo `.apk` para o dispositivo Android
   - Permita instalação de fontes desconhecidas nas configurações
   - Execute o instalador

---

## **Como Usar o Aplicativo**

1. **Inicie o aplicativo** no dispositivo móvel
2. **Mova a câmera** lentamente para detectar superfícies
3. **Toque na tela** para colocar o primeiro ponto de medição
4. **Toque novamente** para colocar o segundo ponto
5. **A distância** será exibida automaticamente
6. **Toque no botão "Reset"** para nova medição

---

## **Resultados e Conclusões**

Este projeto demonstrou a integração bem-sucedida de:
- Tracking de superfícies em tempo real
- Renderização 3D em ambiente real
- Cálculos matemáticos para conversão de unidades
- Interface adaptativa para diferentes dispositivos

As principais dificuldades superadas foram:
- Calibração precisa das medições
- Estabilização dos pontos em superfícies irregulares
- Otimização de performance para dispositivos móveis

---

## **Referências Bibliográficas**

1. Unity Technologies. (2023). ARFoundation Documentation.
2. Apple Developer. (2023). ARKit Framework Guide.
3. Google Developers. (2023). ARCore Overview.
4. Foley, J. D., van Dam, A., Feiner, S. K., & Hughes, J. F. (2014). Computer Graphics: Principles and Practice.

---

## **Licença**

Este projeto foi desenvolvido para fins acadêmicos. O código-fonte é disponibilizado para estudo e referência, com restrições de uso comercial sem autorização prévia.

---

## **Contato**

Para dúvidas ou contribuições, entre em contato com os autores:
- Davi Oliveira Cortes: [davi.cortes@discente.ufma.br]
- Lucas Emanoel Amaral Gomes: [lucas.gomes@discente.ufma.br]

**Universidade Federal do Maranhão**  
**Departamento de Engenharia da Computação**  
**São Luís - MA, 2025**

---

*Projeto desenvolvido como requisito parcial para aprovação na disciplina de Computação Gráfica, UFMA 2025.1*
