# Mapeamento Colaborativo do SIGTAP para vocabulários padronizados do OMOP CDM

## O Projeto
Esse projeto está sendo desenvolvido pela comunidade brasileira para mapeamento dos termos da tabela SIGTAP do SUS para vocabulários padronizados do Modelo Comum de Dados (_CDM_) OMOP.

## Objetivos do Projeto
- Mapear os termos do SIGTAP para vocabulários padronizados
- Educar a comunidade brasileira em relação as ferramentas disponíveis
- Estabelecer governança para contribuições de forma descentralizada
- Ampliar o número de participantes na comunidade OHDSI Brasil/LATAM
- Estimular o conhecimento OMOP para o público da SBIS

## Métricas de Sucesso
- Número de usuários ativos nos fóruns OHDSI em português. Meta: 15 usuários em 6 meses
- % de termos mapeados. Meta: 99% mais utilizados (por faturamento) no prazo de 6 meses

## Fases do Projeto
### Primeira Fase
- Objetivo: engajar a comunidade a participar do projeto de mapeamento
- Resultados: tivemos 117 participantes inscritos

### Segunda Fase
- Objetivos: migração para a plataforma DoltHub

# Roteiro do participante
Siga estas etapas para participar do projeto Sigtap Omop. Clique no link de cada uma.
1. Criar conta no DoltHub e fazer o fork do repositório central. (Entrar)		
2. Instalar os programas necessários através do pacote UDZ.zip. (Instalar)
	
3. Baixar termos para mapear no Usagi. (Baixar)  
		a. Fornece novos termos dentro do limite pré-estabelecido de termos por participante em cada vez.  
		b. Se tentar baixar de novo, após já ter baixado antes, o sistema simplesmente fornece novamente os mesmos termos da última vez.  
		c. Libera novos termos para mapear após receber os mapeamentos dos termos baixados anteriormente.  
	
4. Mapear termos com o Usagi, e salvar (não exportar) o arquivo CSV. (Mapear)
	
5. Fazer upload do arquivo CSV para o DoltHub. (Subir)
	
6. Visualizar ou baixar os mapeamentos acordados até o presente momento. (Ver)
	
7. Escrever comentários, abrir um problema (issue), ou iniciar alguma discussão. (Comentar)
	
8. Obter estatísticas simples atualizadas em tempo real. (Estatísticas)  
		○ Número (e %) de termos mapeados.  
		○ Número (e %) de mapeamentos produzidos.  
		○ Número (e %) de termos atualmente reservados por participantes.  

## Entrar
1. Acessar https://www.dolthub.com/.  
2. Clicar em Sign in.	
3. Clicar em Don't have an account yet? Create one.  
4. Criar conta através de qualquer uma das formas disponíveis.  
5. Uma vez logado, acessar https://www.dolthub.com/repositories/ohdsi-brasil/sigtap_omop.  
6. Clicar em Fork. Confirmar.  

## Instalar
1. Baixar o UDZ.zip:  
	○ Link (Usagi): https://1drv.ms/u/s!Auk_d44Mzjh_vIEAK_KOWDxtztXqdA?e=GpOjx8  
	○ Baixar e descompactar, cada um pode demorar horas.   
	
2. Descompactar na pasta desejada. Essa pasta será o o diretório base. Ela contém:  
	a. usagi/: Usagi pronto para ser usado (índices [vocabulários] pré-construídos).  
	b. dolt/: Dolt e arquivos associados a ele.  
	c. r/: R e script Zelador (zelador.R).  
	d. zelador.bat: Script para executar em Windows.  
	e. zelador.command: Script para executar em Mac.  
	
3. Ir no diretório base e executar o zelador.  
	a. Windows: clicar no zelador.bat.  
	b. Mac: clicar no zelador.command.  
	
4. Zelador perguntará se você quer inicializar o sistema Dolt. Confirmar.  
	
5. Zelador abrirá o navegador.  
	a. Se o navegador ainda não está logado no DoltHub, será preciso fazer login.  
	b. Após login, o site redirecionará automaticamente para a página de criar credenciais de acesso (access token). Inserir qualquer nome (não faz diferença) e salvar.  
	
6. Voltar para o Zelador. Ver que o programa detectou com sucesso a criação das credenciais.
	
7. Aguardar um ou dois minutos para o Zelador confirmar também a clonagem do repositório.