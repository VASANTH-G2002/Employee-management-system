CREATE TABLE [dbo].[Employees] (
    [EmpId]          VARCHAR (20)    NOT NULL,
    [FirstName]      NVARCHAR (100)  NOT NULL,
    [LastName]       NVARCHAR (100)  NULL,
    [Email]          NVARCHAR (255)  NOT NULL,
    [Mobile]         NVARCHAR (20)   NULL,
    [DateOfBirth]    DATE            NULL,
    [Address]        NVARCHAR (255)  NULL,
    [City]           NVARCHAR (100)  NULL,
    [State]          NVARCHAR (100)  NULL,
    [Country]        NVARCHAR (100)  NULL,
    [ZipCode]        NVARCHAR (20)   NULL,
    [ProfileImg]     NVARCHAR (255)  NULL,
    [About]          NVARCHAR (MAX)  NULL,
    [EmployeeStatus] NVARCHAR (50)   NULL,
    [Department]     NVARCHAR (100)  NULL,
    [Designation]    NVARCHAR (100)  NULL,
    [DateOfJoining]  DATE            NULL,
    [ReportingId]    NVARCHAR (20)   NULL,
    [CTC]            DECIMAL (18, 2) NULL,
    [AccountNo]      NVARCHAR (50)   NULL,
    [BankName]       NVARCHAR (100)  NULL,
    [IFSCCode]       NVARCHAR (20)   NULL,
    [Branch]         NVARCHAR (100)  NULL,
    [AccountType]    NVARCHAR (50)   NULL,
    [PasswordHash]   NVARCHAR (200)  NOT NULL,
    [Role]           NVARCHAR (50)   NULL,
    PRIMARY KEY CLUSTERED ([EmpId] ASC),
    UNIQUE NONCLUSTERED ([Email] ASC)
);

Create Database EMS and add table Employees



Table records

EMS1000	John	Doe	john.doe@example.com	9876543210	12-03-1990	123 Main St	New York	NY	USA	10001	NULL	Experienced software engineer specializing in backend development.	Active	IT	Software Engineer	15-05-2020	NULL	75000.00	1234567890	Bank of America	BOFA0001234	NYC Main Branch	Savings	J5n6YQ5bFtEABFhNffmZP+vwLlDda8x3CdX0cAxxfCA=

	User
EMS1001	vasanth	g	vasanth05@gmail.com	9876543211	20-07-1992	456 Park Ave	Los Angeles	CA	USA	90001	Uploads/54336833-8d1c-420a-b8aa-d96f00b2e2c3.png	Front-end developer passionate about UX design.	Active	IT	UI Developer	10-02-2021	EMS1000	68000.00	9876543210	Chase Bank	CHAS0005678	LA Downtown	Savings	lI52jMYQj/D1B4dsSXbuHj0TiWyfzol2t3NKERsPnf4=	Admin
EMS1002	Michael	Brown	michael.brown@example.com	9876543212	15-01-1985	789 Elm St	Chicago	IL	USA	60601		Project manager with 10 years of experience in agile delivery.	Active	Operations	Project Manager	05-09-2018		95000.00	1122334455	Wells Fargo	WF0001111	Chicago Branch	Current	HASHEDPASSWORD3	Manager
EMS1003	Emily	Clark	emily.clark@example.com	9876543213	25-04-1995	321 Oak St	Houston	TX	USA	77001	NULL	HR professional skilled in talent acquisition.	Active	HR	HR Executive	01-03-2022	EMS1002	55000.00	2233445566	Citi Bank	CITI0009999	Houston Central	Savings	HASHEDPASSWORD4	Employee
EMS1004	David	Johnson	david.johnson@example.com	9876543214	05-12-1988	654 Pine St	San Francisco	CA	USA	94101	NULL	Senior engineer with expertise in cloud infrastructure.	Active	IT	DevOps Engineer	12-11-2019	EMS1000	88000.00	3344556677	Bank of America	BOFA0004321	SF Downtown	Current	HASHEDPASSWORD5	Employee
EMS1005	David	Wilson	david.wilson@example.com	9876543215	18-12-1989	900 Market St	Boston	MA	USA	02108	NULL	Backend developer with Python and Django expertise.	Active	IT	Backend Developer	05-08-2020	EMS1002	78000.00	6655443322	TD Bank	TD0004444	Boston Central	Savings	L0pshFQ8d2s3vFv8H2A==	Admin
EMS1006	Emily	Johnson	emily.johnson@example.com	9876543216	09-02-1994	13 Pine St	Austin	TX	USA	73301	NULL	UI/UX designer with strong graphic design skills.	Active	IT	UI/UX Designer	12-03-2023	EMS1003	69000.00	5544332211	Chase Bank	CHAS0009999	Austin HQ	Savings	F3sa1Rts5LpoDa5fQWz==	Admin
EMS1007	Liam	Martinez	liam.martinez@example.com	9876543217	22-07-1990	74 Main Blvd	Denver	CO	USA	80202	NULL	DevOps engineer automating cloud infrastructure.	Active	IT	DevOps Engineer	15-10-2021	EMS1002	83000.00	4433221100	PNC Bank	PNC0008888	Denver South	Savings	Q1dk7Lb5uRpMfd5bGcT==	Admin
EMS1008	Olivia	Anderson	olivia.anderson@example.com	9876543218	17-05-1995	18 Maple Rd	Portland	OR	USA	97201	NULL	Junior software developer learning Go and microservices.	Active	IT	Junior Developer	09-04-2024	EMS1004	62000.00	3322110099	Key Bank	KEY0007777	Portland Main	Savings	N2al6Pe4xRmKcd6cDgL==	Admin
EMS1009	Noah	Garcia	noah.garcia@example.com	9876543219	29-03-1991	77 Broadway	Houston	TX	USA	77002	NULL	Mobile app developer specializing in Flutter.	Active	IT	Mobile Developer	20-09-2020	EMS1003	71000.00	2211009988	Chase Bank	CHAS0005555	Houston Central	Savings	M1vs9Hb4pFtXce7aBgC==	Admin
EMS1010	Ava	Lopez	ava.lopez@example.com	9876543220	11-01-1996	245 Ocean Dr	Miami	FL	USA	33101	NULL	QA engineer ensuring software reliability and performance.	Active	IT	QA Engineer	19-07-2022	EMS1005	67000.00	2200112233	Wells Fargo	WF0009999	Miami Beach	Savings	K7al9Pa7wZrQgf7pTtM==	Admin
EMS1011	Ethan	Thomas	ethan.thomas@example.com	9876543221	09-04-1987	122 Greenway Ln	Atlanta	GA	USA	30301	NULL	Systems analyst with experience in ERP and SAP.	Active	IT	Systems Analyst	22-06-2019	EMS1000	88000.00	8899001122	Regions Bank	REGN0001234	Atlanta Midtown	Savings	R4sj2Np9bXfUhf5vFrB==	Admin
EMS1012	Isabella	Davis	isabella.davis@example.com	9876543222	14-05-1993	96 River Rd	San Diego	CA	USA	92101	NULL	Front-end developer with Vue.js and accessibility focus.	Active	IT	Frontend Developer	10-09-2021	EMS1004	72000.00	3344556677	Chase Bank	CHAS0012345	San Diego West	Savings	Z8js5Uf4nRvJad6bPxN==	Admin
EMS1013	Lucas	Hernandez	lucas.hernandez@example.com	9876543223	05-10-1992	33 Elmwood St	Dallas	TX	USA	75201	NULL	Security engineer specializing in network and endpoint security.	Active	IT	Security Engineer	25-11-2020	EMS1002	94000.00	5566778899	Bank of America	BOFA0006789	Dallas HQ	Savings	D1vh7Lf2tXsHfe6pFjG==	Admin
EMS1014	Charlotte	Martinez	charlotte.martinez@example.com	9876543224	28-12-1994	404 Oak St	Minneapolis	MN	USA	55401	NULL	Project coordinator managing agile software delivery.	Active	PMO	Project Coordinator	15-01-2023	EMS1001	65000.00	9988007766	US Bank	USB0004444	Minneapolis Main	Savings	C2al3Df8qGhMaf5nPpB==	Admin
EMS1015	James	White	james.white@example.com	9876543225	03-03-1989	89 Hillcrest Ave	Phoenix	AZ	USA	85001	NULL	Network administrator maintaining secure connections.	Active	IT	Network Admin	14-03-2020	EMS1003	87000.00	5566998844	Chase Bank	CHAS0008889	Phoenix Downtown	Savings	G3kj8Xe9vCtNje7zWwP==	Admin
EMS1016	Amelia	Robinson	amelia.robinson@example.com	9876543226	19-09-1997	55 Highland Dr	Columbus	OH	USA	43004	NULL	Junior data analyst experienced in SQL and Power BI.	Active	Analytics	Data Analyst	22-03-2024	EMS1005	63000.00	6677889900	PNC Bank	PNC0005678	Columbus Main	Savings	V9pn3Rg5tQeJaf6zLrM==	Admin
EMS1017	Henry	King	henry.king@example.com	9876543227	15-11-1990	144 Cedar Ave	Nashville	TN	USA	37201	NULL	IT support specialist providing end-user technical assistance.	Active	Support	IT Support	03-06-2021	EMS1004	59000.00	7788990011	Regions Bank	REGN0007777	Nashville Central	Savings	H4kd5Tf8vPpOha8rTtN==	Admin
EMS1018	Grace	Perez	grace.perez@example.com	9876543228	08-02-1995	301 Birch Rd	Charlotte	NC	USA	28202	NULL	Business analyst bridging IT and operations.	Active	Business	Business Analyst	08-08-2022	EMS1001	71000.00	8899776655	Wells Fargo	WF0004321	Charlotte Uptown	Savings	P5as8Rf7kHsTib9xJpQ==	Admin
EMS1019	Alexander	Scott	alexander.scott@example.com	9876543229	12-06-1988	90 Redwood Dr	Las Vegas	NV	USA	88901	NULL	Software architect designing scalable enterprise solutions.	Active	IT	Software Architect	05-10-2019	EMS1000	105000.00	9988776655	Chase Bank	CHAS0002345	Vegas Strip	Savings	S6as7Pg6mKtHfe8rWpD==	Admin
EMS1020	Mia	Turner	mia.turner@example.com	9876543230	10-08-1993	501 Palm St	San Jose	CA	USA	95112	NULL	Backend engineer building REST APIs and microservices.	Active	IT	Backend Engineer	11-04-2022	EMS1002	80000.00	5544223311	Wells Fargo	WF0001235	San Jose Downtown	Savings	B8fs3Ng5vLpKge9qUtE==	Admin
EMS1021	Sebastian	Adams	sebastian.adams@example.com	9876543231	21-09-1991	25 Spruce St	Indianapolis	IN	USA	46204	NULL	Data scientist experienced in Python, R, and ML models.	Active	Analytics	Data Scientist	17-10-2020	EMS1005	92000.00	2211334455	Chase Bank	CHAS0003412	Indianapolis Main	Savings	M9lp2Qe7nGsRbf5kTyH==	Admin
EMS1022	Harper	Nelson	harper.nelson@example.com	9876543232	27-07-1994	444 Cypress Ln	Salt Lake City	UT	USA	84101	NULL	Scrum master managing agile development teams.	Active	PMO	Scrum Master	13-02-2021	EMS1001	77000.00	6622334411	US Bank	USB0002121	SLC Downtown	Savings	Q7ad5Wg6tRtKac4pJxN==	Admin
EMS1023	Daniel	Ramirez	daniel.ramirez@example.com	9876543233	30-10-1989	170 Bay St	Tampa	FL	USA	33602	NULL	Full-stack developer with Java and Angular expertise.	Active	IT	Full Stack Developer	12-08-2019	EMS1003	85000.00	9988221144	Regions Bank	REGN0006677	Tampa Main	Savings	K4vj6Re3pHxNda7rWvS==	Admin
EMS1024	Ella	Young	ella.young@example.com	9876543234	05-11-1995	321 Lake St	Kansas City	MO	USA	64101	NULL	IT recruiter focusing on software and data roles.	Active	HR	IT Recruiter	01-05-2023	EMS1000	68000.00	2233445566	Bank of America	BOFA0001115	KC Central	Savings	T3aq8De4nVrKgd5tYwL==	Admin
EMS1025	Benjamin	Wright	benjamin.wright@example.com	9876543235	18-01-1990	88 Willow Ave	Raleigh	NC	USA	27601	NULL	Cloud architect with experience in Kubernetes and AWS.	Active	IT	Cloud Architect	22-12-2020	EMS1002	99000.00	6677884411	Wells Fargo	WF0004567	Raleigh HQ	Savings	V5ls9Jt4yDsHef8rBpP==	Admin
EMS1026	Scarlett	Hill	scarlett.hill@example.com	9876543236	14-02-1992	15 Maple Ave	Cleveland	OH	USA	44101	NULL	Marketing analyst measuring campaign effectiveness.	Active	Marketing	Marketing Analyst	10-03-2022	EMS1001	64000.00	7788992211	PNC Bank	PNC0002345	Cleveland Main	Savings	Y4ap6Qg7tWxJhf6pLvM==	Admin
EMS1027	Jack	Campbell	jack.campbell@example.com	9876543237	25-05-1987	501 Lincoln Rd	Orlando	FL	USA	32801	NULL	Infrastructure engineer focused on automation and monitoring.	Active	IT	Infrastructure Engineer	04-09-2018	EMS1000	91000.00	5544667788	Chase Bank	CHAS0008901	Orlando East	Savings	R2mk7Hg5vLtPcd4qWnN==	Admin
EMS1028	Chloe	Mitchell	chloe.mitchell@example.com	9876543238	12-10-1996	22 Park Blvd	Baltimore	MD	USA	21201	NULL	Software tester ensuring high-quality web releases.	Active	QA	QA Tester	05-07-2023	EMS1004	62000.00	4433221166	Wells Fargo	WF0007654	Baltimore Downtown	Savings	P3zl9Kj8mVrGbc6tFqT==	Admin
EMS1029	Logan	Green	logan.green@example.com	9876543239	22-12-1989	302 Cherry St	Detroit	MI	USA	48201	NULL	Software developer maintaining internal enterprise tools.	Active	IT	Software Developer	19-06-2020	EMS1003	78000.00	3322445566	Bank of America	BOFA0007777	Detroit HQ	Savings	J8fs6Lp4nBtMhf5vZrQ==	Admin
EMS1030	Victoria	Bennett	victoria.bennett@example.com	9876543240	17-04-1991	145 Cedar St	Omaha	NE	USA	68102	NULL	HR manager with experience in employee engagement programs.	Active	HR	HR Manager	25-03-2021	EMS1001	85000.00	6677993322	US Bank	USB0005555	Omaha Central	Savings	H2nf6Qr9mRtDhe7vXpC==	Admin
EMS1031	Samuel	Murphy	samuel.murphy@example.com	9876543241	05-08-1988	310 Grand Ave	Tulsa	OK	USA	74103	NULL	Software engineer focusing on API design and development.	Active	IT	Software Engineer	10-11-2019	EMS1002	87000.00	4455667788	Chase Bank	CHAS0003123	Tulsa HQ	Savings	B5pa8Fd4sHwJgf8rKxT==	Admin
EMS1032	Luna	Foster	luna.foster@example.com	9876543242	29-07-1996	41 Ocean View Rd	San Antonio	TX	USA	78205	NULL	UX researcher gathering insights for better design.	Active	IT	UX Researcher	11-08-2023	EMS1004	70000.00	5544336677	Wells Fargo	WF0006543	San Antonio North	Savings	T6ps7Ng3xUvLbe6vRrD==	Admin
EMS1033	Aiden	Cook	aiden.cook@example.com	9876543243	01-10-1992	210 Pinecrest Blvd	Pittsburgh	PA	USA	15222	NULL	Business intelligence developer using Tableau and SQL.	Active	Analytics	BI Developer	02-12-2021	EMS1005	83000.00	7788995544	PNC Bank	PNC0009999	Pittsburgh HQ	Savings	M8dl6He9tFrPcd6sLpB==	Admin
EMS1034	Layla	Richardson	layla.richardson@example.com	9876543244	18-09-1993	80 Pearl St	Buffalo	NY	USA	14201	NULL	Technical writer documenting software APIs and guides.	Active	IT	Technical Writer	14-05-2022	EMS1003	66000.00	6655884411	Bank of America	BOFA0009998	Buffalo North	Savings	K9er5Qh6rFsNhe8yLpP==	Admin
EMS1035	Wyatt	Bailey	wyatt.bailey@example.com	9876543245	24-06-1989	612 Ridge Rd	Louisville	KY	USA	40202	NULL	Systems engineer specializing in Linux servers.	Active	IT	Systems Engineer	07-07-2019	EMS1002	88000.00	9988774433	Regions Bank	REGN0005555	Louisville HQ	Savings	L4jh8Xs7tHpQef7tWrF==	Admin
EMS1036	Zoey	Patterson	zoey.patterson@example.com	9876543246	03-02-1997	71 Forest Ln	Richmond	VA	USA	23219	NULL	Junior QA tester assisting automation efforts.	Active	QA	QA Tester	15-01-2024	EMS1004	58000.00	3322115566	Wells Fargo	WF0004568	Richmond Main	Savings	V3pl9Jr6wFsMge6uTrN==	Admin
EMS1037	Elijah	Cox	elijah.cox@example.com	9876543247	11-12-1990	200 Market Blvd	Boise	ID	USA	83702	NULL	Lead DevOps engineer with Kubernetes experience.	Active	IT	Lead DevOps Engineer	28-09-2020	EMS1003	96000.00	7788996655	Chase Bank	CHAS0002234	Boise Downtown	Savings	F5dn6Qe8yGrLhf5zVtQ==	Admin
EMS1038	Aria	Hughes	aria.hughes@example.com	9876543248	09-03-1995	31 Laurel Dr	Milwaukee	WI	USA	53202	NULL	Software tester focusing on regression automation.	Active	QA	QA Engineer	20-06-2022	EMS1005	71000.00	5544337766	US Bank	USB0007778	Milwaukee East	Savings	C9ds4Ng7pHsJge8qRpL==	Admin
EMS1039	Hannah	Bryant	hannah.bryant@example.com	9876543249	23-01-1994	450 Birch St	Albuquerque	NM	USA	87101	NULL	Software engineer developing microservice APIs.	Active	IT	Software Engineer	08-04-2021	EMS1001	76000.00	2211445577	Wells Fargo	WF0006544	Albuquerque Main	Savings	N8gs3Kq5rFwMdf8tYpB==	Admin
EMS1040	Matthew	Watson	matthew.watson@example.com	9876543250	16-05-1988	90 Elm Ave	Reno	NV	USA	89501	NULL	Product manager with experience in agile SaaS development.	Active	Product	Product Manager	22-05-2019	EMS1000	95000.00	9988223344	Chase Bank	CHAS0005567	Reno Main	Savings	R7ak8Df9wGtJfe7sXpM==	Admin
EMS1041	Nora	Howard	nora.howard@example.com	9876543251	14-08-1992	221 Elmwood Ave	Madison	WI	USA	53703	NULL	HR coordinator assisting with onboarding and training.	Active	HR	HR Coordinator	10-09-2022	EMS1001	60000.00	2233441122	US Bank	USB0003336	Madison Central	Savings	G6ls7We4xJtMgf8vTpN==	Admin
EMS1042	Carter	Reed	carter.reed@example.com	9876543252	21-02-1990	68 Riverbend Rd	Anchorage	AK	USA	99501	NULL	Systems administrator managing network infrastructure.	Active	IT	Systems Administrator	18-07-2020	EMS1003	88000.00	6677885522	Wells Fargo	WF0007888	Anchorage Main	Savings	T5nh8Dp6yFqKfe8wYrQ==	Admin
EMS1043	Penelope	Bell	penelope.bell@example.com	9876543253	27-11-1995	37 Highland Ave	Des Moines	IA	USA	50309	NULL	Marketing coordinator supporting digital campaigns.	Active	Marketing	Marketing Coordinator	08-03-2023	EMS1001	64000.00	4455778899	Bank of America	BOFA0005543	Des Moines HQ	Savings	J4rk5Hf8vGmLcd7uTpP==	Admin
EMS1044	Leo	Griffin	leo.griffin@example.com	9876543254	10-12-1991	402 Maple Rd	Tucson	AZ	USA	85701	NULL	IT support technician handling software issues.	Active	Support	IT Support Technician	09-05-2021	EMS1004	59000.00	7788993322	Chase Bank	CHAS0007776	Tucson Main	Savings	L7vs9Df7zXcHjg9pQrL==	Admin
EMS1045	Stella	Long	stella.long@example.com	9876543255	19-01-1993	19 Oakwood Blvd	Cincinnati	OH	USA	45202	NULL	Software developer specializing in Java and Spring Boot.	Active	IT	Software Developer	20-02-2022	EMS1003	78000.00	5566778890	PNC Bank	PNC0003333	Cincinnati HQ	Savings	K5ap8Df6xVnLge9sXrQ==	Admin
EMS1046	Hudson	Evans	hudson.evans@example.com	9876543256	07-03-1987	70 Pine St	Riverside	CA	USA	92501	NULL	Solutions architect designing enterprise applications.	Active	IT	Solutions Architect	25-02-2019	EMS1000	102000.00	3344556678	Wells Fargo	WF0009995	Riverside HQ	Savings	P8ks7Rf8wGnMdf6vJtS==	Admin
EMS1047	Eleanor	Price	eleanor.price@example.com	9876543257	15-06-1994	33 Woodland Dr	Birmingham	AL	USA	35203	NULL	Data engineer developing ETL pipelines and data flows.	Active	Analytics	Data Engineer	30-08-2021	EMS1005	89000.00	2211335599	Regions Bank	REGN0002233	Birmingham HQ	Savings	N6yr8Pf9sGlJhf7rQvM==	Admin
EMS1048	Zoe	Barnes	zoe.barnes@example.com	9876543258	02-10-1996	299 Maple Ave	Lincoln	NE	USA	68508	NULL	Junior developer maintaining legacy applications.	Active	IT	Junior Developer	18-09-2023	EMS1004	61000.00	6677998800	US Bank	USB0004569	Lincoln Central	Savings	B3ks9Fg6tVrKde8xLpP==	Admin
EMS1049	Owen	Henderson	owen.henderson@example.com	9876543259	04-04-1989	520 Harbor St	Providence	RI	USA	02903	NULL	Senior software developer with .NET and cloud experience.	Active	IT	Senior Developer	12-11-2020	EMS1002	95000.00	7788992210	Bank of America	BOFA0008765	Providence HQ	Savings	S7nl8Qe7vLpKfe9pYrC==	Admin
NULL	NULL	NULL	NULL	NULL	NULL	NULL	NULL	NULL	NULL	NULL	NULL	NULL	NULL	NULL	NULL	NULL	NULL	NULL	NULL	NULL	NULL	NULL	NULL	NULL	NULL
