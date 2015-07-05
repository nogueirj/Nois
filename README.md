# Nois
___________________________________________________________________________________________________________________
Como ter lucro?
___________________________________________________________________________________________________________________
Qual as posicões dos menus e o que vai aparecer?
___________________________________________________________________________________________________________________
Gastos com o hospedam e com o boleto para o fornecedor do serviço?
___________________________________________________________________________________________________________________
Ver quanto ao contador, questões de cnpj, custo sobre o serviço ofertado e custos para abrir um cnpj?
___________________________________________________________________________________________________________________
QUestões quanto ao banco e conta?
___________________________________________________________________________________________________________________
Quem somos e como trabalhamos?
___________________________________________________________________________________________________________________
Ver quantos aos aplicativos da google?
___________________________________________________________________________________________________________________
Ofertas e Sorteios:
Como vai ser, para nos mesmos.

___________________________________________________________________________________________________________________
<b>BANCO DE DADOS - TABELAS - NORMALIZAÇÃO</b>

PLACES:</br>
  t.string :phone </br>
  t.string :site</br>
  t.string :description</br>
  t.string :name</br>
  t.string :edited, default: 0</br>
  t.string :authorized, default: 0</br>
  t.string :location</br>
  t.datetime :deleted_at</br>
  t.references :category</br>
  t.references :user</br>
  t.attachment :photo  </br>
  
OFFERS:

USERS:</br>
  t.string :email,              null: false, default: ""</br>
  t.string :encrypted_password, null: false, default: ""</br>
  t.string   :reset_password_token</br>
  t.datetime :reset_password_sent_at</br>
  t.datetime :remember_created_at</br>
  t.integer  :sign_in_count, default: 0, null: false</br>
  t.datetime :current_sign_in_at</br>
  t.datetime :last_sign_in_at</br>
  t.string   :current_sign_in_ip</br>
  t.string   :last_sign_in_ip</br>
  t.boolean :locked, default: 0</br>
  t.string :name</br>
  t.string :phone, default: ""</br>
  t.string :mobile, default: ""</br>
  t.string :city, default: ""</br>
  t.string :state, default: ""</br>
  t.string :country, default: "Brasil"
  t.string :business, default: ""</br>
  t.boolean :anonymous, default: 0</br>
  t.boolean :admin, default: 0</br>
      
PRIZES:

MESSAGES:</br>
  t.string :name</br>
	t.string :email</br>
	t.string :mobile</br>
	t.string :phone</br>
	t.text :subject</br>
  t.datetime :deleted_at</br>

NEWSLETTERS:</br>
  t.string :email</br>
  
COMMENTS:</br>
  t.string :name</br>
	t.text :texto</br>
	t.string :email</br>
	t.references :place</br>
	t.datetime :deleted_at</br>
	
CATEGORIES:</br>
  t.string :name</br>
	t.string :description</br>
	t.datetime :deleted_at</br>
	t.attachment :photo</br>
	
SUBCATEGORIES:</br>
  t.string :name</br>
	t.references :category</br>
	t.datetime :deleted_at</br>
	
SYSTEM_CONFIGS:</br>
  t.string :email</br>
	t.boolean :systemlocked, default: 0</br>
___________________________________________________________________________________________________________________


