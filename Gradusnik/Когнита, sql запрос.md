#### -запрос на назначенные вопросы и ответа  админа магазина, когнита

`select * from grad_five_min_edu_answers`
`where uf_user_id = 322 and` 
	`year(uf_datetime) = 2025 and` 
	`month(uf_datetime) = 12 and` 
	`(uf_status is NULL or`
	`uf_status = 82)`


#### -запрос на удаление ответов  админа магазина, когнита 

`DELETE from grad_five_min_edu_answers`
`where uf_user_id = 322 and` 
	`year(uf_datetime) = 2025 and` 
	`month(uf_datetime) = 12 and` 
	`(uf_status is NULL or`
	 uf_status = 82)


код ответа когнита:
	80 - неверно
	79 - верно
	82 - игнор
	NULL - нет ответа