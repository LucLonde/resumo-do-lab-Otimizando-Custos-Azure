# Resumo do laboratório de Otimizando Custos no Azure

Gerenciar custos no Azure é fundamental para otimizar os gastos e garantir que os recursos sejam utilizados de maneira eficiente. O Azure oferece diversas ferramentas e práticas que podem ajudar a monitorar, controlar e reduzir os custos. Aqui estão algumas abordagens e práticas recomendadas para o gerenciamento e otimização de custos no Azure:

### 1. **Azure Cost Management and Billing**
   O **Azure Cost Management and Billing** é a principal ferramenta integrada que permite:
   - **Monitorar os gastos em tempo real:** Acompanhe o uso de recursos e os custos associados.
   - **Definir alertas e orçamentos:** Configure orçamentos para controlar os gastos e receba alertas quando os limites forem atingidos.
   - **Analisar o consumo:** Relatórios detalhados ajudam a entender como os serviços estão sendo utilizados e onde estão os maiores custos.
   - **Distribuir custos por departamento ou projeto:** Isso permite alocar os custos de maneira precisa, facilitando a análise e a responsabilidade sobre o orçamento.

### 2. **Utilização de Reservas (Azure Reservations)**
   - **Reservas de VM:** Adquirir máquinas virtuais reservadas por 1 ou 3 anos oferece descontos significativos em comparação com o pagamento por uso (pay-as-you-go).
   - **Reservas de banco de dados e outros serviços:** O Azure também oferece reservas para serviços como SQL Database, Cosmos DB e outros.

### 3. **Aproveitar o Azure Hybrid Benefit**
   - Se você já possui licenças do Windows Server ou SQL Server com Software Assurance, pode utilizar o **Azure Hybrid Benefit** para economizar em custos de licenciamento no Azure. Isso pode reduzir os custos de execução de máquinas virtuais Windows e bancos de dados SQL.

### 4. **Identificar e Eliminar Recursos Ociosos ou Subutilizados**
   - **Máquinas virtuais não utilizadas:** Desligue ou exclua máquinas virtuais que estão rodando sem carga.
   - **Dimensionamento correto:** Garanta que os recursos estão dimensionados adequadamente para as necessidades da aplicação. Em muitos casos, uma máquina menor pode suportar a carga adequadamente, reduzindo custos.
   - **Escalonamento automático (auto-scaling):** Configure o **auto-scaling** para ajustar automaticamente os recursos com base na demanda, evitando o desperdício de capacidade durante períodos de baixa demanda.

### 5. **Usar Níveis de Serviço Adequados**
   - Para muitos serviços no Azure, existem diferentes níveis de serviço (tiers), como **Standard**, **Premium**, e **Basic**. Verifique se suas necessidades realmente exigem os níveis mais altos, ou se um nível inferior pode atender aos requisitos com menor custo.

### 6. **Gerenciamento de Custos com Tags**
   - Utilize **tags** para categorizar os recursos com base em projetos, departamentos, ou ambientes (produção, desenvolvimento, etc.). Isso facilita a análise de custos por projeto e a identificação de áreas que precisam de otimização.
   
### 7. **Dimensionar corretamente o armazenamento e redes**
   - **Armazenamento:** Verifique se os discos estão sendo utilizados adequadamente, e utilize os níveis de armazenamento otimizados para o custo (por exemplo, **Cool** ou **Archive Blob** para dados raramente acessados).
   - **Transferência de dados:** Minimizar a transferência de dados entre regiões e otimize o uso de redes internas para reduzir custos.

### 8. **Aproveitar Serviços Gerenciados**
   Em vez de gerenciar manualmente infraestrutura complexa (como bancos de dados ou balanceadores de carga), usar serviços gerenciados do Azure, como **Azure SQL Database** ou **App Service**, pode reduzir o tempo de administração e otimizar os custos.

### 9. **Economia com Escalonamento e Otimização de Workloads**
   - **Escalonamento horizontal vs. vertical:** Adotar escalonamento horizontal (adicionar mais instâncias menores) pode ser mais eficiente que o escalonamento vertical (aumentar o tamanho da máquina).
   - **Agendamento de desligamento automático:** Configure scripts ou utilize ferramentas nativas para desligar recursos não essenciais durante horários de inatividade (como à noite ou em finais de semana).

### 10. **Aplicação de Descontos e Incentivos**
   O Azure oferece uma série de programas de descontos e incentivos, como o **Azure Dev/Test Pricing**, que fornece descontos para ambientes de desenvolvimento e teste. Verifique se sua organização pode se qualificar para esses programas.

### 11. **Usar o Azure Advisor**
   O **Azure Advisor** é uma ferramenta que analisa seu ambiente e fornece recomendações para melhorar a eficiência de custos, desempenho, segurança e confiabilidade. Ele pode identificar recursos subutilizados, sugerir otimizações de dimensionamento e destacar oportunidades para uso de reservas e licenças.

### 12. **Containerização e Kubernetes**
   Utilizar contêineres com **Azure Kubernetes Service (AKS)** pode ajudar a otimizar o uso de infraestrutura, aumentando a eficiência do uso de recursos e reduzindo os custos associados ao gerenciamento de múltiplas máquinas virtuais.

### 13. **Uso de Spot VMs**
   As **Spot VMs** do Azure oferecem capacidade de computação a preços significativamente mais baixos em troca da possibilidade de interrupção quando o Azure precisa da capacidade. São ideais para cargas de trabalho que podem lidar com interrupções.

### Conclusão:
Ao implementar essas práticas, você pode gerenciar e otimizar seus custos no Azure de forma eficaz. O uso de ferramentas integradas, como o **Cost Management**, o monitoramento contínuo e a otimização de recursos podem reduzir os custos e aumentar a eficiência no ambiente Azure.
