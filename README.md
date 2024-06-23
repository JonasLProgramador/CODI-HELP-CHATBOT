<!DOCTYPE html>
<html lang="pt-BR">

<body>
    <div class="container">
        <h1>CODI-HELP</h1>
        <p>Bem-vindo ao projeto <strong>CODI-HELP</strong>! Este projeto tem a iniciativa de criar um chatbot que realiza tarefas cotidianas para os estudantes da <strong>Programadores do Amanhã (PDA)</strong>. Ele pode fornecer cronogramas, mini-mapas e mais. Além disso, o bot integra a inteligência artificial <strong>Gemini</strong> para responder a perguntas complexas que o bot padrão da PDA pode não conseguir.</p>
        <h2>Sumário</h2>
        <ul>
            <li><a href="#visao-geral">Visão Geral</a></li>
            <li><a href="#estrutura-do-projeto">Estrutura do Projeto</a></li>
            <li><a href="#configuracao">Configuração e Execução</a></li>
            <li><a href="#funcionalidades">Funcionalidades Principais</a></li>
            <li><a href="#dependencias">Dependências</a></li>
            <li><a href="#licenca">Licença</a></li>
        </ul>
        <h2 id="visao-geral">Visão Geral</h2>
        <p>O <strong>CODI-HELP</strong> é um bot do Discord projetado para ajudar estudantes da <strong>Programadores do Amanhã</strong> (PDA) com diversas tarefas. Ele responde a comandos específicos e pode alternar entre dois modos:</p>
        <ul>
            <li><strong>Modo PDA:</strong> Fornece cronogramas, mini-mapas e informações relacionadas ao curso.</li>
            <li><strong>Modo Gemini:</strong> Utiliza a IA <strong>Gemini</strong> da Google para responder a perguntas mais complexas.</li>
        </ul>
        <h2 id="estrutura-do-projeto">Estrutura do Projeto</h2>
        <p>A estrutura principal do projeto é a seguinte:</p>
        <pre><code>
/
├── mapas/
│   ├── mapaIn.pdf
│   ├── mapaPg.pdf
│   └── mapaSt.pdf
├── cronogramas/
│   └── cronograma.pdf
├── .env
├── server.js
└── package.json
        </code></pre>
        <p><strong>Nota:</strong> Certifique-se de ter os arquivos PDF corretos em suas respectivas pastas.</p>
        <h2 id="configuracao">Configuração e Execução</h2>
        <p>Siga as instruções abaixo para configurar e executar o <strong>CODI-HELP</strong> localmente:</p>
        <ol>
            <li>Clone o repositório:</li>
            <pre><code>git clone https://github.com/JonasLeiteProgramador/CODI-HELP.git</code></pre>
            <li>Instale as dependências:</li>
            <pre><code>npm install</code></pre>
            <li>Crie um arquivo <code>.env</code> no diretório raiz com o seguinte conteúdo:</li>
            <pre><code>
# .env
TOKEN=seu-token-do-discord
API_KEY=token-gerado-pelo-google-apis
            </code></pre>
            <li>Substitua <code>seu-token-do-discord</code> pelo seu token de bot do Discord e <code>token-gerado-pelo-google-apis</code> pela sua chave da API Gemini.</li>
            <li>Inicie o bot:</li>
            <pre><code>node server.js</code></pre>
        </ol>
        <h2 id="funcionalidades">Funcionalidades Principais</h2>
        <p>O <strong>CODI-HELP</strong> possui as seguintes funcionalidades:</p>
        <ul>
            <li><strong>Saudações e Perguntas:</strong> Responde a saudações comuns e perguntas sobre o estado do bot.</li>
            <li><strong>Fornecimento de Mini-Mapas:</strong> Envia mini-mapas de soft skills, inglês e programação.</li>
            <li><strong>Fornecimento de Cronogramas:</strong> Envia o cronograma do curso.</li>
            <li><strong>Arremates:</strong> Fornece links para os arremates.</li>
            <li><strong>Justificativa de Faltas:</strong> Fornece o link para justificar faltas.</li>
            <li><strong>Modo Gemini:</strong> Alterna para usar a IA Gemini para responder perguntas mais complexas.</li>
        </ul>
        <p>Você pode alternar entre o bot PDA e o Gemini usando um botão na interface do Discord.</p>
        <h2 id="dependencias">Dependências</h2>
        <p>As principais dependências deste projeto são:</p>
        <ul>
            <li><a href="https://discord.js.org/" target="_blank">Discord.js</a> - Biblioteca para interagir com a API do Discord.</li>
            <li><a href="https://www.npmjs.com/package/dotenv" target="_blank">dotenv</a> - Biblioteca para carregar variáveis de ambiente.</li>
            <li><a href="https://developers.generative-ai.google" target="_blank">Google Generative AI</a> - Biblioteca para integrar com a IA Gemini da Google.</li>
        </ul>
        <p>Veja a lista completa de dependências no arquivo <code>package.json</code>.</p>
        <h2 id="licenca">Licença</h2>
        <p>Este projeto é licenciado sob a Licença MIT. Consulte o arquivo <a href="LICENSE">LICENSE</a> para obter mais detalhes.</p>
        <p>Esperamos que você aproveite e contribua com o <strong>CODI-HELP</strong>! Se você encontrar problemas ou tiver sugestões, sinta-se à vontade para abrir uma issue ou enviar um pull request.</p>
    </div>
</body>
</html>
