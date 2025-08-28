# 📊 AcompanhAqui - Documentação do Projeto

## 🎯 Visão Geral do Projeto

O **AcompanhAqui** é um sistema web para acompanhamento de performance de equipes de vendas, desenvolvido para facilitar o controle de indicadores, metas e resultados de forma visual e intuitiva.

---

## 📋 Levantamento de Requisitos

### 🔧 Requisitos Funcionais

#### RF01 - Sistema de Login
- O sistema deve permitir que usuários façam login informando nome e loja
- Os dados do usuário devem ser armazenados para personalização da experiência
- Após o login, o usuário deve ser direcionado para a página principal

#### RF02 - Dashboard Principal (Welcome)
- Exibir boas-vindas personalizadas com o nome do usuário
- Mostrar ranking da equipe ordenado por performance (pays)
- Apresentar indicadores principais: Pay Mês, Pay Semana e NPS
- Calcular automaticamente diferenças entre metas e resultados
- Destacar os 3 melhores performers da semana

#### RF03 - Acompanhamento por Semanas (Ranking Loja)
- Organizar dados por semanas específicas (SW32, SW33, SW34, SW35)
- Separar indicadores por categorias: PAY, PCJ, SEGUROS, CPF/PTC/SNIPER
- Calcular automaticamente saldo/débito (real - meta)
- Aplicar cores visuais baseadas na performance
- Mostrar detalhes de promotores e detratores com tooltips

#### RF04 - Página de Indicadores Editáveis (ICP)
- Permitir edição de dados através de interface web
- Implementar sistema de autenticação para modo administrador
- Controlar acesso com senha para edições
- Salvar alterações automaticamente

#### RF05 - Sistema de Navegação
- Menu de navegação fixo entre as páginas
- Botões de retorno para navegação intuitiva
- Interface responsiva para diferentes dispositivos

### 🎨 Requisitos Não Funcionais

#### RNF01 - Usabilidade
- Interface intuitiva e fácil de usar
- Cores e indicadores visuais claros
- Tooltips informativos ao passar o mouse
- Design responsivo para mobile e desktop

#### RNF02 - Performance
- Carregamento rápido das páginas
- Animações suaves e transições
- Cálculos automáticos em tempo real

#### RNF03 - Segurança
- Controle de acesso para funcionalidades administrativas
- Validação de senha para modo de edição
- Armazenamento seguro de dados do usuário

#### RNF04 - Compatibilidade
- Funcionar em navegadores modernos
- Suporte a dispositivos móveis
- Interface adaptável a diferentes tamanhos de tela

---

## 👤 Histórias de Usuário

### 🏠 Módulo de Login

**História 1: Acesso ao Sistema**
> **Como** funcionário da empresa  
> **Eu quero** fazer login informando meu nome e loja  
> **Para que** eu possa acessar meus dados de performance personalizados

**Critérios de Aceite:**
- ✅ Campos obrigatórios: Nome e Loja
- ✅ Dados salvos para uso nas próximas páginas
- ✅ Redirecionamento automático após login
- ✅ Interface simples e clara

---

### 📊 Módulo Dashboard Principal

**História 2: Visualização de Performance Pessoal**
> **Como** funcionário logado  
> **Eu quero** ver minha posição no ranking da equipe  
> **Para que** eu saiba como estou performando comparado aos colegas

**Critérios de Aceite:**
- ✅ Ranking ordenado por número de pays
- ✅ Exibição de nome, loja, pays e variável
- ✅ Destaque visual para as 3 primeiras posições
- ✅ Atualização automática dos dados

**História 3: Acompanhamento de Metas**
> **Como** funcionário  
> **Eu quero** ver se estou atingindo minhas metas mensais e semanais  
> **Para que** eu possa ajustar minha estratégia de vendas

**Critérios de Aceite:**
- ✅ Indicadores de Pay Mês, Pay Semana e NPS
- ✅ Comparação automática entre meta e real
- ✅ Cores diferentes para saldo positivo (verde) e negativo (vermelho)
- ✅ Cálculo automático de diferenças

---

### 📈 Módulo Acompanhamento Semanal

**História 4: Análise por Períodos**
> **Como** gestor ou funcionário  
> **Eu quero** analisar a performance por semanas específicas  
> **Para que** eu possa identificar tendências e padrões

**Critérios de Aceite:**
- ✅ Abas separadas para cada semana (SW32, SW33, SW34, SW35)
- ✅ Dados organizados por categorias de indicadores
- ✅ Navegação fácil entre as semanas
- ✅ Scroll horizontal para visualização em telas menores

**História 5: Detalhamento de Promotores e Detratores**
> **Como** gestor  
> **Eu quero** ver detalhes dos promotores e detratores  
> **Para que** eu possa reconhecer bons performers e apoiar quem precisa

**Critérios de Aceite:**
- ✅ Nomes separados em colunas individuais
- ✅ Tooltips com informações de volume e conversão
- ✅ Hover interativo para mostrar detalhes
- ✅ Dados independentes para cada pessoa

**História 6: Visualização de Status por Cores**
> **Como** usuário  
> **Eu quero** identificar rapidamente o status das metas através de cores  
> **Para que** eu não precise ler números para entender a situação

**Critérios de Aceite:**
- ✅ Verde para saldo positivo e posições 1-3
- ✅ Amarelo para posições 4-6
- ✅ Vermelho para saldo negativo e posições 7+
- ✅ Aplicação consistente em todo o sistema

---

### ⚙️ Módulo Administrativo (ICP)

**História 7: Controle de Acesso**
> **Como** administrador do sistema  
> **Eu quero** controlar quem pode editar os dados  
> **Para que** apenas pessoas autorizadas façam alterações

**Critérios de Aceite:**
- ✅ Pergunta inicial sobre acesso administrativo
- ✅ Validação de senha para modo de edição
- ✅ Modo somente leitura para usuários comuns
- ✅ Mensagens claras sobre o tipo de acesso

**História 8: Edição de Indicadores**
> **Como** administrador autorizado  
> **Eu quero** editar os dados dos indicadores diretamente na web  
> **Para que** eu possa manter as informações sempre atualizadas

**Critérios de Aceite:**
- ✅ Células clicáveis para edição
- ✅ Salvamento automático das alterações
- ✅ Feedback visual das mudanças
- ✅ Botão para confirmar salvamento

**História 9: Navegação Entre Páginas**
> **Como** usuário do sistema  
> **Eu quero** navegar facilmente entre as diferentes páginas  
> **Para que** eu possa acessar todas as funcionalidades sem dificuldade

**Critérios de Aceite:**
- ✅ Botão de voltar em todas as páginas
- ✅ Menu de navegação fixo
- ✅ Links funcionais entre as seções
- ✅ Interface consistente em todas as páginas

---

## 🏗️ Arquitetura do Sistema

### 📁 Estrutura de Arquivos
```
projeto-trae/
├── index.html          # Página de login
├── welcome.html        # Dashboard principal
├── ranking-loja.html   # Acompanhamento semanal
├── icp.html           # Indicadores editáveis
├── styles.css         # Estilos globais
└── DOCUMENTACAO.md    # Esta documentação
```

### 🔄 Fluxo de Navegação
1. **Login** (index.html) → Usuário informa nome e loja
2. **Dashboard** (welcome.html) → Visualiza ranking e indicadores
3. **Acompanhamento** (ranking-loja.html) → Analisa dados por semana
4. **ICP** (icp.html) → Edita indicadores (se autorizado)

### 💾 Armazenamento de Dados
- **LocalStorage**: Dados do usuário logado
- **JavaScript**: Dados dos indicadores e rankings
- **CSS**: Configurações visuais e responsividade

---

## 🎨 Design e Interface

### 🌈 Paleta de Cores
- **Azul Principal**: #1a237e (navegação e títulos)
- **Verde**: Saldos positivos e boas posições
- **Vermelho**: Saldos negativos e posições baixas
- **Amarelo**: Posições médias
- **Cinza**: Elementos neutros

### 📱 Responsividade
- Design adaptável para desktop, tablet e mobile
- Scroll horizontal para tabelas em telas pequenas
- Botões e elementos com tamanho adequado para touch
- Fontes e espaçamentos otimizados para cada dispositivo

---

## 🚀 Funcionalidades Implementadas

### ✅ Concluídas
- [x] Sistema de login com armazenamento local
- [x] Dashboard com ranking da equipe
- [x] Indicadores com cálculo automático
- [x] Sistema de abas por semanas
- [x] Tooltips informativos
- [x] Controle de acesso administrativo
- [x] Interface responsiva
- [x] Sistema de cores por performance
- [x] Navegação entre páginas
- [x] Edição de dados via web

### 🔄 Melhorias Futuras
- [ ] Integração com banco de dados
- [ ] Relatórios em PDF
- [ ] Gráficos interativos
- [ ] Notificações push
- [ ] Histórico de alterações
- [ ] Backup automático

---

## 👥 Perfis de Usuário

### 🧑‍💼 Funcionário Comum
- Acessa dados pessoais e da equipe
- Visualiza rankings e indicadores
- Não pode editar informações
- Foco em acompanhamento de performance

### 👨‍💻 Administrador
- Todos os acessos do funcionário comum
- Pode editar dados dos indicadores
- Controla informações da equipe
- Responsável por manter dados atualizados

### 📊 Gestor
- Visualiza dados de toda a equipe
- Analisa tendências e padrões
- Usa informações para tomada de decisão
- Acompanha metas e resultados

---

## 📞 Suporte e Manutenção

Para dúvidas, sugestões ou problemas técnicos:
- Verifique se todos os arquivos estão no mesmo diretório
- Certifique-se de que o navegador suporta JavaScript
- Em caso de problemas, recarregue a página (Ctrl+F5)
- Para edições, use sempre o modo administrador

---

*Documentação criada em: Dezembro 2024*  
*Versão: 1.0*  
*Sistema: AcompanhAqui - Acompanhamento de Performance*