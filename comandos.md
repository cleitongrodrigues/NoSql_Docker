## db.alunos.insertMany([{nome: "Ana"}]) --// usado para inserir registros  

## db.alunos.updateOne({nome: 'Ester'}, {$set: {ativo: false}}) --// usado para atualizar um registro

## db.alunos.deleteOne({nome: 'Ana'}) --// usado para remover um registro

## db.alunos.find() --// usado para fazer consultas

## $gt --// Serve para pegar valores numéricos que sejam mais que ex: db.alunos.find({idade : {$gt:20}})

## $gte --// Serve para pegar valores numéricos que sejam menores ou iguais a ex: db.alunos.find({idade : {$gte:20}})

## $lt --// Serve para pegar valores numéricos que sejam menores que ex: db.alunos.find({idade : {$lt:22}})

## $lte --// Serve para pegar valores numéricos que sejam menores ou igual a ex: db.alunos.find({idade : {$lte:22}})

## Combinação para buscar um aluno com idade entre 18 a 22 ex: db.alunos.find({idade : {$gte:18, $lte:22}})

## $ne --// Buscar o que seja diferente de ex: db.alunos.find({curso : {$ne: 'ADS'}})

## $in --// Buscar registros que estejam entre algo. Ex: db.alunos.find({periodo: {$in:['manha','tarde']}})

## $nin --// Buscar registros que não estejam entre algo. Ex: db.alunos.find({periodo: {$nin:['manha','tarde']}})

## $and db.alunos.find({$and: [{curso: 'DSM'}, {periodo: 'manha'}]}) --// Operador lógico and

## $or db.alunos.find({$or: [{curso: 'DSM'}, {periodo: 'manha'}]}) --// Operador lógico or