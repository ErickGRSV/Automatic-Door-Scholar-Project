# Requisitos do Sistema

## 1. Objetivo

Desenvolver um sistema de controle de acesso por biometria para controlar
a entrada de funcionários autorizados na área interna da gestão escolar.

## 2. Escopo

O sistema deverá:

- Cadastrar funcionários autorizados.
- Cadastrar e gerenciar biometrias.
- Validar o acesso por biometria.
- Liberar a porta após autenticação válida.
- Permitir abertura manual em situações excepcionais.
- Registrar tentativas de acesso.
- Bloquear o dispositivo após 5 tentativas inválidas.
- Emitir sinais através de LED e buzzer.
- Funcionar na rede local.

O sistema não deverá controlar:

- Visitantes.
- Alunos.
- Funcionários temporários.

## 3. Requisitos Funcionais

| ID | Requisito |
|---|---|
| RF01 | Cadastrar funcionários autorizados. |
| RF02 | Cadastrar CPF e biometria. |
| RF03 | Editar dados e biometria. |
| RF04 | Excluir funcionários. |
| RF05 | Autenticar usuários por biometria. |
| RF06 | Liberar a porta após autenticação válida. |
| RF07 | Permitir abertura manual. |
| RF08 | Gerenciar permissões administrativas. |
| RF09 | Permitir cadastro pela Diretoria de Serviços. |
| RF10 | Permitir permissões secundárias. |
| RF11 | Emitir confirmação sonora através do buzzer. |
| RF12 | Permitir funcionamento sem internet através da rede local. |
| RF13 | Registrar tentativas inválidas. |
| RF14 | Bloquear após 5 tentativas inválidas. |
| RF15 | Acionar alarme após tentativas inválidas. |
| RF16 | Manter o dispositivo bloqueado até liberação manual. |
| RF17 | Permitir futura implementação de campainha por sala. |

## 4. Requisitos Não Funcionais

| ID | Requisito |
|---|---|
| RNF01 | Funcionamento das 06h00 às 00h00. |
| RNF02 | Alta disponibilidade durante o horário de funcionamento. |
| RNF03 | Funcionamento na rede local sem depender da internet. |
| RNF04 | Possuir alternativa de abertura em caso de falha elétrica. |
| RNF05 | Equipamento instalado na parede. |
| RNF06 | Fácil utilização pelos administradores. |
| RNF07 | Armazenamento seguro das informações biométricas. |
| RNF08 | Permitir manutenção por profissionais de tecnologia. |
| RNF09 | A porta permanece aberta pelo lado interno. |
| RNF10 | Interface gráfica poderá ser implementada futuramente. |

## 5. Regras de Negócio

- Aproximadamente 150–170 funcionários terão acesso inicialmente.
- Apenas funcionários fixos serão cadastrados.
- O sistema funcionará das 06h00 às 00h00.
- A Diretoria de Serviços será responsável pelo cadastro e gerenciamento.
- Diretores e coordenadores poderão possuir permissões secundárias.
- Após 5 tentativas inválidas, o dispositivo será bloqueado.
- A abertura manual deverá existir para situações excepcionais.
- Em caso de falta de energia, deverá existir uma alternativa física de acesso.

## 6. Componentes do Sistema

### Controle de acesso
- Sensor biométrico
- ESP
- Fechadura elétrica
- LED vermelho
- LED verde
- Buzzer
- Botão de abertura manual

### Software
- Sistema embarcado
- Servidor/API
- Banco de dados

## 7. Questões Pendentes

- Modelo definitivo do sensor biométrico.
- Local de armazenamento da biometria.
- Forma de cadastro da biometria.
- Necessidade de criptografia e método utilizado.
- Estratégia definitiva para funcionamento offline.
- Definição do mecanismo de abertura em caso de falta de energia.
- Definição sobre a interface administrativa.
