# Guia de Uso e Manutenção

Este documento fornece instruções detalhadas sobre como utilizar, manter e atualizar seu perfil profissional no Instagram e sua página web de apresentação.

## Índice
1. [Configuração Inicial](#configuração-inicial)
2. [Perfil do Instagram](#perfil-do-instagram)
3. [Página Web](#página-web)
4. [Hospedagem no GitHub Pages](#hospedagem-no-github-pages)
5. [Integração entre Plataformas](#integração-entre-plataformas)
6. [Manutenção e Atualizações](#manutenção-e-atualizações)
7. [Monitoramento de Resultados](#monitoramento-de-resultados)
8. [Solução de Problemas](#solução-de-problemas)

## Configuração Inicial

### Arquivos do Projeto
Todos os arquivos necessários estão organizados na seguinte estrutura:
```
portfolio/
├── css/
│   └── style.css
├── js/
│   └── script.js
├── img/
│   └── (suas imagens)
├── index.html
├── estrategia_instagram.md
├── orientacoes_foto_perfil.md
├── modelo_biografia_instagram.md
├── exemplos_publicacoes_instagram.md
├── integracao_instagram_web.md
└── guia_uso_manutencao.md (este documento)
```

### Requisitos Técnicos
- Conta no GitHub para hospedagem da página web
- Conta no Instagram para configuração do perfil profissional
- Editor de código para manutenção dos arquivos (recomendado: Visual Studio Code)
- Conhecimentos básicos de HTML, CSS e JavaScript para atualizações

## Perfil do Instagram

### Configuração Inicial do Perfil
1. **Foto de Perfil**:
   - Siga as orientações detalhadas no arquivo `orientacoes_foto_perfil.md`
   - Use uma foto profissional que transmita credibilidade e competência técnica
   - Mantenha o mesmo estilo visual da sua página web para consistência

2. **Biografia**:
   - Utilize um dos modelos fornecidos no arquivo `modelo_biografia_instagram.md`
   - Personalize conforme suas preferências, mantendo o foco em sistemas de vendas, controle de estoque e desenvolvimento web/app
   - Adicione o link para sua página web hospedada no GitHub Pages

3. **Primeiras Publicações**:
   - Siga o plano de conteúdo detalhado no arquivo `exemplos_publicacoes_instagram.md`
   - Publique os 9 posts iniciais ao longo de 3 semanas (3 por semana)
   - Mantenha consistência visual em todas as publicações

### Manutenção do Perfil
1. **Frequência de Postagem**:
   - Mantenha uma frequência regular (2-3 posts por semana)
   - Use o Instagram Stories diariamente para manter engajamento

2. **Tipos de Conteúdo**:
   - Alterne entre os diferentes tipos de conteúdo sugeridos na estratégia
   - Atualize seu portfólio com novos projetos à medida que os desenvolve
   - Compartilhe dicas técnicas e tendências do mercado

3. **Engajamento**:
   - Responda a todos os comentários em suas publicações
   - Interaja com perfis relevantes da sua área
   - Participe de discussões em hashtags relacionadas à sua especialidade

## Página Web

### Navegação e Estrutura
A página web está organizada nas seguintes seções:
1. **Hero (Início)**: Apresentação inicial com chamada para ação
2. **Sobre**: Informações pessoais e profissionais
3. **Habilidades**: Competências técnicas organizadas por categorias
4. **Projetos**: Portfólio de trabalhos com filtros por categoria
5. **Contato**: Formulário e informações para contato

### Personalização de Conteúdo
Para atualizar o conteúdo da página:

1. **Informações Pessoais**:
   - Edite o arquivo `index.html` nas seções correspondentes
   - Atualize textos de apresentação na seção "Sobre"
   - Modifique informações de contato na seção "Contato"

2. **Habilidades**:
   - Ajuste os níveis de habilidades no HTML modificando os valores de largura nos elementos com classe `skill-level`
   - Adicione novas habilidades seguindo o mesmo padrão HTML existente

3. **Projetos**:
   - Para adicionar um novo projeto, copie o bloco HTML de um projeto existente e modifique:
     ```html
     <div class="project-card" data-category="categoria">
         <div class="project-image">
             <div class="project-placeholder">
                 <i class="fas fa-icon"></i>
             </div>
         </div>
         <div class="project-info">
             <h3>Nome do Projeto</h3>
             <p>Descrição do projeto.</p>
             <div class="project-tech">
                 <span>Tecnologia 1</span>
                 <span>Tecnologia 2</span>
             </div>
             <div class="project-links">
                 <a href="#" class="btn-small"><i class="fas fa-eye"></i> Ver Demo</a>
                 <a href="#" class="btn-small"><i class="fab fa-github"></i> Código</a>
             </div>
         </div>
     </div>
     ```
   - Atualize o atributo `data-category` para que o filtro funcione corretamente

4. **Imagens**:
   - Substitua a imagem de perfil placeholder por sua foto profissional
   - Adicione screenshots de seus projetos na pasta `img/`
   - Atualize os caminhos das imagens no HTML

## Hospedagem no GitHub Pages

### Configuração Inicial
1. **Criar Repositório**:
   - Acesse sua conta no GitHub e crie um novo repositório
   - Nome recomendado: `seu-usuario.github.io` (para site pessoal)
   - Alternativa: qualquer nome de repositório (para projeto)

2. **Upload de Arquivos**:
   - Clone o repositório para sua máquina local:
     ```
     git clone https://github.com/seu-usuario/seu-repositorio.git
     ```
   - Copie todos os arquivos da pasta `portfolio/` para o repositório clonado
   - Faça commit e push das alterações:
     ```
     git add .
     git commit -m "Primeira versão do portfólio"
     git push origin main
     ```

3. **Ativar GitHub Pages**:
   - Acesse as configurações do repositório no GitHub
   - Na seção "GitHub Pages", selecione a branch principal (main ou master)
   - Salve as configurações e aguarde alguns minutos para a publicação

### URL do Site
- Se você usou o formato `seu-usuario.github.io`, seu site estará disponível em `https://seu-usuario.github.io/`
- Se usou outro nome, estará em `https://seu-usuario.github.io/nome-do-repositorio/`

## Integração entre Plataformas

### Link do Instagram para a Página Web
1. **Configurar Link na Bio**:
   - Acesse seu perfil do Instagram
   - Clique em "Editar perfil"
   - Cole a URL do seu site no campo "Site"
   - Salve as alterações

2. **Mencionar o Site nas Publicações**:
   - Inclua frases como "Link na bio para mais detalhes" em suas publicações
   - Crie stories destacando seções específicas do seu site

### Link da Página Web para o Instagram
Os links para suas redes sociais já estão configurados na seção de contato da página web. Para atualizá-los:

1. **Editar Links**:
   - Abra o arquivo `index.html`
   - Localize a seção com os links sociais:
     ```html
     <div class="social-links">
         <a href="https://instagram.com/seu_perfil" class="social-link" title="Instagram">
             <i class="fab fa-instagram"></i>
         </a>
         <!-- outros links sociais -->
     </div>
     ```
   - Substitua `seu_perfil` pelo seu nome de usuário real no Instagram

## Manutenção e Atualizações

### Atualizações Regulares
Para manter seu perfil profissional relevante:

1. **Página Web**:
   - Adicione novos projetos à medida que os desenvolve
   - Atualize suas habilidades conforme aprende novas tecnologias
   - Revise textos e informações de contato periodicamente

2. **Instagram**:
   - Siga o plano de conteúdo estabelecido na estratégia
   - Atualize suas publicações com novos projetos e aprendizados
   - Mantenha-se atualizado com tendências do setor

### Backup de Arquivos
- Mantenha uma cópia local de todos os arquivos do projeto
- Use o próprio GitHub como sistema de backup
- Considere criar branches para testar novas funcionalidades antes de publicá-las

## Monitoramento de Resultados

### Métricas do Instagram
Monitore regularmente:
- Crescimento de seguidores
- Engajamento por publicação (curtidas, comentários, salvamentos)
- Visitas ao perfil
- Cliques no link da bio

### Métricas da Página Web
Para acompanhar o desempenho do seu site:
1. **Configurar Google Analytics**:
   - Crie uma conta no Google Analytics
   - Adicione o código de rastreamento ao seu HTML
   - Monitore visitantes, tempo de permanência e páginas mais acessadas

2. **Formulário de Contato**:
   - Acompanhe o número de mensagens recebidas
   - Analise a conversão de visitantes em contatos

## Solução de Problemas

### Problemas Comuns e Soluções

1. **Página Web Não Atualiza Após Alterações**:
   - Verifique se fez commit e push das alterações para o GitHub
   - Limpe o cache do navegador (Ctrl+F5 ou Cmd+Shift+R)
   - Aguarde alguns minutos para a propagação das alterações

2. **Elementos Visuais Quebrados**:
   - Verifique os caminhos dos arquivos CSS e JavaScript
   - Confirme se todas as imagens foram carregadas corretamente
   - Teste a página em diferentes navegadores

3. **Formulário de Contato Não Funciona**:
   - O formulário atual é uma simulação e não envia mensagens reais
   - Para implementar um formulário funcional, considere usar serviços como Formspree ou Netlify Forms

4. **Problemas de Responsividade**:
   - Teste a página em diferentes dispositivos e tamanhos de tela
   - Ajuste o CSS conforme necessário para corrigir problemas específicos

### Recursos Adicionais
- [Documentação do GitHub Pages](https://docs.github.com/pt/pages)
- [Guia do Instagram para Empresas](https://business.instagram.com/getting-started)
- [Documentação HTML/CSS/JavaScript (MDN)](https://developer.mozilla.org/pt-BR/docs/Web)

---

Este guia foi criado para ajudá-lo a gerenciar e manter seu perfil profissional no Instagram e sua página web de apresentação. Para dúvidas adicionais ou suporte, entre em contato com o desenvolvedor.
