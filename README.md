🔐 Login Automatizado com Selenium e Excel

Este projeto realiza o login automatizado em um sistema web utilizando dados extraídos de uma planilha Excel. A automação é feita com Selenium, e o processo é iniciado por uma interface gráfica com Tkinter.

⚙️ Funcionalidades
- Interface gráfica com Tkinter
- Leitura de credenciais e ambiente a partir de uma planilha Excel
- Login automatizado em sistema web via Selenium
- Registro de logs para acompanhamento do processo

🛠️ Pré-requisitos
- Python 3 instalado
- Instalar as bibliotecas necessárias:
  ```bash
  pip install selenium openpyxl
  ```
- Ter o ChromeDriver compatível com sua versão do Google Chrome
- Arquivo `planilha.xlsx` com os dados nas células:
  - `A2`: Login
  - `B2`: Senha
  - `C2`: Ambiente

📁 Estrutura esperada da planilha

| Login       | Senha       | Ambiente   |
|-------------|-------------|------------|
| usuario123  | senha123    | Producao   |

🚀 Como usar
1. Configure a URL do sistema web no trecho `driver.get('https://')`.
2. Certifique-se de que o arquivo `planilha.xlsx` esteja no mesmo diretório do script ou ajuste o caminho.
3. Execute o script:
   ```bash
   python processo1.py
   ```
4. Uma janela será exibida informando o sucesso do processo.

⚠️ Observações
- O script fecha o navegador automaticamente após a execução.
- Em caso de erro, uma mensagem será exibida e o log será registrado no console.
- Para ambientes com autenticação multifator ou CAPTCHA, será necessário adaptar o código.

📄 Licença
Este projeto é de uso interno e não possui uma licença pública definida.
