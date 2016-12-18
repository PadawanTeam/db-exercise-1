#Iniciando os testes com Mongo

=======================================

###Inserindo as cervejas(E criando a collection)

'''javascript
db.cervejas.insert([{
	nome:'Heineken',
	garrafaLata:'Long Neck',
	tipo:'Pilsen',
	paisOrigem:'Bélgica',
	preco:6.99,
	sabor:'Malte Forte',
	cor:'Clara',
	aromatizada:'Não',
	premiada:'Sim',
	gourmet:'Não'
},{
	nome:'Kremmer',
	garrafaLata:'Copo',
	tipo:'Chopp',
	paisOrigem:'Inferno',
	preco:2.99,
	sabor:'Horrivel',
	cor:'Clara',
	aromatizada:'Não',
	premiada:'Não',
	gourmet:'Não'
}])
'''

###Selecionando a collection e vendo os resultados:

'''javascript
> db.cervejas.find()
{ "_id" : ObjectId("5856fed84b5807ff7c76fd23"), "nome" : "Heineken", "garrafaLata" : "Long Neck", "tipo" : "Pilsen", "paisOrigem" : "Bélgica", "preco" : 6.99, "sabor" : "Malte Forte", "cor" : "Clara", "aromatizada" : "Não", "premiada" : "Sim", "gourmet" : "Não" }
{ "_id" : ObjectId("5856fed84b5807ff7c76fd24"), "nome" : "Kremmer", "garrafaLata" : "Copo", "tipo" : "Chopp", "paisOrigem" : "Inferno", "preco" : 2.99, "sabor" : "Horrivel", "cor" : "Clara", "aromatizada" : "Não", "premiada" : "Não", "gourmet" : "Não" }
'''
_______________________________________________________________

###Criando a collection de lanches (E inserindo os lanches)

'''javascript
db.lanches.insert([{
	nome:'VinaBurguer',
	principal:'Hamburguer de Vina',
	molho:'Barbecue',
	salada:'Cebola e Alface',
	preco:16.99,
	pao:'Cacetinho',
	tostado:'sim',
	apimentado:'Opcional',
	caramelizado:'cebola e picles',
	gourmet:'sim'
},{
	nome:'Big Mc',
	principal:'2 Hamburgueres de carne',
	molho:'Especial',
	salada:'Alface - cebola',
	preco:15.99,
	pao:'Com Gergelin',
	tostado:'Não',
	apimentado:'Não',
	caramelizado:'Não',
	gourmet:'Não'
}])
'''

###Selecionando a collection e vendo os resultados:

'''javascript
> db.lanches.find()
{ "_id" : ObjectId("5856fd73072c8862846dac77"), "nome" : "VinaBurguer", "principal" : "Hamburguer de Vina", "molho" : "Barbecue", "salada" : "Cebola e Alface", "preco" : 16.99, "pao" : "Cacetinho", "tostado" : "sim", "apimentado" : "Opcional", "caramelizado" : "cebola e picles", "gourmet" : "sim" }
{ "_id" : ObjectId("5856fd73072c8862846dac78"), "nome" : "Big Mc", "principal" : "2 Hamburgueres de carne", "molho" : "Especial", "salada" : "Alface - cebola", "preco" : 15.99, "pao" : "Com Gergelin", "tostado" : "Não", "apimentado" : "Não", "caramelizado" : "Não", "gourmet" : "Não" }
'''
