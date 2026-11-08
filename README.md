# Laboratório com Kali Linux e Medusa

## Sobre o projeto

Este projeto foi desenvolvido como parte de um desafio prático da Digital Innovation One (DIO), com o objetivo de estudar vulnerabilidades relacionadas à autenticação e compreender os riscos de senhas fracas em serviços de rede e aplicações web.

A atividade foi realizada em um ambiente de laboratório controlado, utilizando Kali Linux, Medusa, Metasploitable 2 e DVWA.

Durante os testes, foram explorados cenários de auditoria de autenticação, identificação de serviços, enumeração de usuários e validação de credenciais.

## Objetivos

- Compreender o funcionamento de ataques de força bruta e password spraying.
- Conhecer a ferramenta Medusa e suas aplicações em auditorias de segurança.
- Identificar serviços e portas disponíveis em um ambiente de laboratório.
- Avaliar os riscos associados ao uso de senhas fracas.
- Identificar vulnerabilidades relacionadas à autenticação.
- Estudar medidas de prevenção e fortalecimento da segurança.

## Ambiente utilizado

| Componente | Descrição |
|---|---|
| Kali Linux | Sistema operacional utilizado para os testes |
| Medusa | Ferramenta de auditoria de autenticação |
| Metasploitable 2 | Máquina virtual vulnerável para laboratório |
| DVWA | Aplicação web intencionalmente vulnerável |
| VirtualBox | Plataforma de virtualização |
| Rede | Ambiente isolado de laboratório |

## Etapas desenvolvidas

### 1. Configuração do ambiente

Criação das máquinas virtuais no VirtualBox e configuração da comunicação entre os ambientes de laboratório.
<img width="675" height="172" alt="vm" src="https://github.com/user-attachments/assets/1b57870a-80dc-4cce-b94a-82993d6b6cdb" />


### 2. Reconhecimento e identificação de serviços

Verificação da conectividade entre as máquinas e identificação dos serviços disponíveis no ambiente de testes.
<img width="1273" height="687" alt="ip e ping ao metasploitable" src="https://github.com/user-attachments/assets/06305be0-403d-4f6f-9e14-f8eda8d6f52c" />
<img width="1271" height="691" alt="quais portas estão abertas" src="https://github.com/user-attachments/assets/ebed2714-88d7-4919-9467-311f7d7fde29" />


### 3. Enumeração de usuários

Estudo da identificação de contas existentes e dos riscos associados à exposição de informações de usuários.
<img width="1352" height="683" alt="criando arquivo com possiveis senhas e testando se algumas delas bate com o usuario" src="https://github.com/user-attachments/assets/4f1e95e1-1d39-4207-b6c0-265bc59f6643" />


### 4. Auditoria de autenticação no DVWA

Realização de testes controlados em formulário de autenticação da aplicação DVWA, observando o comportamento do sistema diante de tentativas de acesso.
<img width="1313" height="653" alt="descobriu a senha dvwa" src="https://github.com/user-attachments/assets/79d11f3f-232a-4330-bd32-0036d6d886b6" />



### 5. Auditoria de autenticação com Medusa

Estudo da ferramenta Medusa e realização de testes nos serviços disponibilizados pelo ambiente vulnerável, incluindo FTP e SMB.
<img width="862" height="525" alt="medusa encontrou uma credicial valida para o smb" src="https://github.com/user-attachments/assets/dbd4d09e-9e7e-4d03-bf4e-5d25e2bc689a" />


Também foi estudado o conceito de password spraying e os riscos de utilização de credenciais previsíveis.

## Evidências práticas

Os registros das etapas realizadas estão disponíveis na pasta `images/`, contendo capturas de tela do ambiente e dos resultados obtidos durante o laboratório.

## Principais aprendizados

- Importância da identificação e monitoramento de serviços de rede.
- Riscos relacionados a senhas fracas e reutilizadas.
- Funcionamento de ferramentas de auditoria de autenticação.
- Importância da proteção de contas de usuários.
- Importância da documentação de testes e evidências técnicas.

## Recomendações de segurança

Com base nos conceitos estudados, algumas medidas importantes para reduzir os riscos identificados são:

- Utilizar senhas fortes e exclusivas.
- Implementar autenticação multifator (MFA).
- Aplicar políticas de bloqueio ou limitação de tentativas de autenticação.
- Monitorar tentativas de acesso suspeitas.
- Desabilitar serviços desnecessários.
- Restringir o acesso aos serviços por meio de regras de firewall.
- Evitar a exposição de informações sobre contas de usuários.
- Manter sistemas e aplicações atualizados.

## Considerações finais

A realização deste laboratório proporcionou uma experiência prática com ferramentas utilizadas em auditorias de segurança, permitindo compreender melhor os riscos associados aos mecanismos de autenticação.


**Projeto desenvolvido para fins educacionais, exclusivamente em ambiente de laboratório controlado.**

## Referências

- [Kali Linux](https://www.kali.org/)
- [Medusa](http://www.foofus.net/jmk/medusa/medusa.html)
- [DVWA](https://github.com/digininja/DVWA)
- [Nmap](https://nmap.org/)
- [Digital Innovation One](https://www.dio.me/)

## 👩‍💻 Author
Érika Henrichs Ribeiro da Cruz

Focused on **Cybersecurity and Network Infrastructure**.

* LinkedIn: www.linkedin.com/in/érika-cruz-7a97a9344
* GitHub: https://github.com/ErikaCruz96
