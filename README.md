# Vizinho Indica

## Sobre o Projeto

O Vizinho Indica é uma plataforma hiperlocal de recomendações de profissionais e prestadores de serviços baseada na confiança da comunidade.

A proposta é simples:

Ao invés de procurar profissionais em anúncios genéricos ou marketplaces nacionais, os usuários encontram recomendações feitas por moradores do próprio bairro.

O objetivo é transformar perguntas recorrentes dos grupos de WhatsApp em uma experiência organizada, confiável e acessível.

Exemplos:

- "Alguém conhece um eletricista de confiança?"
- "Preciso de uma diarista para esta semana."
- "Quem vocês indicam para instalar ar-condicionado?"

---

# Problema

Todos os dias milhares de moradores perguntam em grupos de WhatsApp e redes sociais por indicações de profissionais.

As dificuldades mais comuns são:

- Falta de confiança em anúncios online.
- Avaliações falsas.
- Profissionais sem referências locais.
- Informações espalhadas em grupos e conversas.

As recomendações mais valiosas geralmente vêm de vizinhos e moradores próximos.

---

# Solução

Criar uma plataforma onde moradores possam:

- Encontrar profissionais recomendados.
- Avaliar serviços contratados.
- Compartilhar experiências reais.
- Descobrir os profissionais mais confiáveis da região.

---

# Objetivo do MVP

Validar a hipótese:

> Moradores confiam mais em recomendações feitas por pessoas do próprio bairro do que em anúncios tradicionais.

---

# Indicadores de Sucesso

## Primeiros 30 dias

- 100 moradores cadastrados
- 50 profissionais cadastrados
- 150 avaliações realizadas
- 1000 buscas realizadas
- Primeiros profissionais interessados em destaque pago

---

# Público-alvo

## Moradores

Pessoas que procuram serviços locais.

Exemplos:

- Eletricistas
- Encanadores
- Diaristas
- Pedreiros
- Pintores
- Chaveiros
- Jardineiros
- Técnicos de informática

---

## Prestadores de Serviço

Profissionais autônomos que dependem de reputação e indicação.

---

# Proposta de Valor

"Encontre profissionais de confiança recomendados pelos seus próprios vizinhos."

---

# Princípio Norteador

A confiança da comunidade vale mais que publicidade.

A plataforma deve priorizar recomendações reais acima de anúncios pagos.

---

# Funcionalidades do MVP

## 1. Busca de Profissionais

Permitir que usuários pesquisem por:

- Categoria
- Cidade
- Bairro

Exemplos:

- Eletricista
- Diarista
- Pintor

---

## 2. Perfil do Profissional

Cada profissional possui:

- Nome
- Foto
- Categoria
- Telefone
- WhatsApp
- Bairro
- Cidade
- Avaliação média
- Quantidade de recomendações

---

## 3. Recomendações

Moradores podem recomendar profissionais.

Dados coletados:

- Nota de 1 a 5 estrelas
- Comentário
- Data da avaliação

---

## 4. Sistema de Avaliação

Exemplo:

⭐⭐⭐⭐⭐

Nota 4.9

Baseado em 23 recomendações.

---

## 5. Listagem por Popularidade

Ordenação por:

- Melhor avaliação
- Mais recomendados
- Mais recentes

---

# Fluxo do Morador

## Primeiro Acesso

1. Criar conta.
2. Informar cidade.
3. Informar bairro.
4. Acessar página principal.

---

## Procurando um Profissional

1. Escolher categoria.
2. Visualizar lista de profissionais.
3. Abrir perfil.
4. Avaliar comentários.
5. Entrar em contato via WhatsApp.

---

## Após Contratar o Serviço

1. Retornar ao sistema.
2. Avaliar profissional.
3. Compartilhar experiência.

---

# Fluxo do Profissional

## Cadastro

1. Criar conta.
2. Escolher categoria.
3. Informar localização.
4. Adicionar foto.
5. Publicar perfil.

---

## Gestão do Perfil

Permitir editar:

- Telefone
- WhatsApp
- Descrição
- Área de atendimento
- Foto

---

# Painel Administrativo

## Dashboard

Indicadores:

- Usuários cadastrados
- Profissionais cadastrados
- Avaliações realizadas
- Bairros ativos

---

## Gestão de Profissionais

Permitir:

- Aprovar cadastro
- Editar informações
- Bloquear perfil
- Destacar profissional

---

## Gestão de Avaliações

Permitir:

- Aprovar avaliação
- Excluir conteúdo inadequado
- Investigar denúncias

---

## Gestão de Categorias

Criar e editar:

- Eletricista
- Encanador
- Pintor
- Diarista
- Pedreiro
- Chaveiro

---

## Gestão de Bairros

Cadastrar:

- Estado
- Cidade
- Bairro

---

# Regras de Negócio

- Usuário precisa estar autenticado para avaliar.
- Um usuário pode avaliar um profissional apenas uma vez.
- Profissionais bloqueados não aparecem nas buscas.
- Avaliações removidas não entram no cálculo da nota.
- Profissionais com menos de três avaliações não recebem selo de destaque.

---

# Sistema de Reputação

## Bronze

5 recomendações

## Prata

20 recomendações

## Ouro

50 recomendações

## Destaque do Bairro

Profissional mais recomendado da região.

---

# Banco de Dados

## Users

- id
- nome
- email
- telefone
- cidade
- bairro
- created_at

---

## Professionals

- id
- nome
- categoria
- telefone
- whatsapp
- descricao
- cidade
- bairro
- foto
- nota_media
- status

---

## Reviews

- id
- user_id
- professional_id
- nota
- comentario
- created_at

---

## Categories

- id
- nome

---

## Neighborhoods

- id
- cidade
- bairro

---

# Design

## Paleta de Cores

### Azul Profissional

#1E3A8A

### Azul Secundário

#2563EB

### Laranja Destaque

#F97316

### Verde Sucesso

#22C55E

### Fundo

#F8FAFC

### Texto

#1F2937

---

# Stack Sugerida

Frontend

- React
- TailwindCSS

Backend

- Supabase

Banco de Dados

- PostgreSQL

Autenticação

- Supabase Auth

Armazenamento

- Supabase Storage

Integrações

- WhatsApp
- Google Maps

---

# Validação Inicial

## Hipótese

Moradores preferem contratar profissionais recomendados pela comunidade local.

## Teste

Lançar em apenas um bairro.

Objetivo:

- 50 profissionais
- 100 moradores
- 200 avaliações

---

# Entregável Esperado do Lovable

Gerar:

- Estrutura completa do MVP
- Navegação entre páginas
- Banco de dados
- Sistema de autenticação
- Sistema de avaliações
- Dashboard administrativo
- Interface responsiva
- Integração com Supabase

---

# Tom de Comunicação

- Próximo
- Humano
- Confiável
- Comunitário
- Simples
- Direto

Evitar linguagem corporativa excessiva.

O aplicativo deve parecer uma recomendação de vizinho e não um marketplace tradicional.
