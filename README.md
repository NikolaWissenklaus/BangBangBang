# 🐔 BangBangBang (Android)

Uma ferramenta de automação baseada em **Streamlit** para capturar e visualizar logs do Google Analytics 4 (GA4) e Firebase em tempo real, diretamente de um dispositivo Android via USB.

Ideal para validação de disparos de eventos de Data Analytics sem a necessidade de ferramentas complexas de proxy.

## 🚀 Pré-requisitos

* **Python 3.14+** instalado.
* **Cabo USB** para conexão de dados.
* **Celular Android** com o aplicativo alvo instalado.

## ⚙️ Configuração do Dispositivo (Android)

Para que a automação consiga ler os logs, você precisa habilitar a depuração:

1.  Vá em **Configurações** > **Sobre o telefone**.
2.  Toque em **Número da versão** (Build Number) 7 vezes até aparecer a mensagem "Você agora é um desenvolvedor".
3.  Volte para **Configurações** > **Sistema** > **Opções do Desenvolvedor**.
4.  Ative a opção **Depuração por USB** (USB Debugging).
5.  Conecte o celular ao PC via USB.

## 📦 Instalação

Abra seu terminal na pasta do projeto e instale as dependências:

```bash
pip install streamlit
```

Mover o arquivo app.py para a pasta com o ADB.
(para instalar o ADB basta acessar o seguinte link: https://developer.android.com/tools/releases/platform-tools?hl=pt-br)

## ▶️ Como Executar
Com o celular conectado e desbloqueado (aceite a permissão de depuração na tela do celular se aparecer):

Execute o comando:
```bash
python -m streamlit run app.py
```
O navegador abrirá automaticamente exibindo os logs e eventos do GA4 capturados do Firebase.



