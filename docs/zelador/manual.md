---
layout: page
title: Script Zelador
subtitle: Manual de Instruções
description: Informações sobre a configuração e uso do script zelador para mapeamento do SIGTAP para OMOP
permalink: /zelador/manual/
menubar: menu_zelador
show_sidebar: false
---

## Manual de Instruções
# Roteiro do participante
Siga estas etapas para participar do mapeamento dos códigos do SIGTAP para os vocabulários do padrão OMOP Common Data Model.
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

## Instalar
3. Ir no diretório base e executar o zelador.  
	a. Windows: clicar no zelador.bat.  
	b. Mac: clicar no zelador.command.  
	
4. Zelador perguntará se você quer inicializar o sistema Dolt. Confirmar.  
	
5. Zelador abrirá o navegador.  
	a. Se o navegador ainda não está logado no DoltHub, será preciso fazer login.  
	b. Após login, o site redirecionará automaticamente para a página de criar credenciais de acesso (access token). Inserir qualquer nome (não faz diferença) e salvar.  
	
6. Voltar para o Zelador. Ver que o programa detectou com sucesso a criação das credenciais.
	
7. Aguardar um ou dois minutos para o Zelador confirmar também a clonagem do repositório.

## Baixar
1. Ir no diretório base e executar o zelador.  
	a. Windows: clicar no zelador.bat.  
	b. Mac: clicar no zelador.command.  
	
2. Escolher opção pega_linhas. Zelador perguntará quantas linhas. Digitar número e apertar Enter.  
	a. Limite: 10 a de 50 de cada vez.  
		
3. Zelador pedirá confirmação para abrir o navegador. Confirmar. O navegador abre na página https://www.dolthub.com/repositories/fabkury/sigtap_omop/pulls/new?refName=main.  
	a. Caso não abra, entrar nesse link manualmente.  
	
4. Participante preenche manualmente:  
	a. Base branch: main  
	b. From branch: main  
	c. Title: [N] linhas reservadas. Substituir [N] pelo número de linhas escolhidas no passo 2.  
	d. Description: em branco ou à vontade do participante.  

5. Clicar em "Create pull request" para executar a operação.  
	a. Esta é a operação de reserva de linhas, que notifica o grupo que o participante decidiu iniciar trabalho nas linhas solicitadas.  
	b. Se quiser pode fechar o navegador após concluir.  
  
Zelador criará diretório base/baixa/linhas_[id].csv, com as linhas para abrir no Usagi.

## Mapear
1. Abrir o Usagi (arquivo JAR na pasta ./Usagi/).  
	
2. Abrir (não importar) o arquivo linhas_[id].csv no Usagi.  
	
3. Fazer o mapeamento.  
	
4. Salvar.  
		
5. Repetir quantas vezes quiser.  

## Subir
1. Ir no diretório base e executar o zelador  
	a. Windows: clicar no zelador.bat.  
	b. Mac: clicar no zelador.command.  
	
2. Escolher a opção sobe_linhas.  
	a. O programa listará os arquivos Usagi detectados.  
	b. Escolher o arquivo linhas_[id].csv que foi usado.  
	
3. Zelador faz o upload das linhas para o DoltHub.  
	
4. Zelador perguntará se pode abrir o navegador. Confirmar.  
	
5. O navegador abre na página https://www.dolthub.com/repositories/fabkury/sigtap_omop/pulls/new?refName=main. O participante preenche:  
	a. Base branch: main  
	b. From branch: main  
	c. Title: à vontade do participante.  
	d. Description: em branco ou à vontade do participante.  
	
6. Clicar Create pull request para executar a operação.