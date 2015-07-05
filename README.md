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

PLACES:
  t.string :phone
  t.string :site
  t.string :description
  t.string :name
  t.string :edited, default: 0
  t.string :authorized, default: 0
  t.string :location
  t.datetime :deleted_at
  t.references :category
  t.references :user
  t.attachment :photo  
  
OFFERS:

USERS:
  t.string :email,              null: false, default: ""
  t.string :encrypted_password, null: false, default: ""
  t.string   :reset_password_token
  t.datetime :reset_password_sent_at
  t.datetime :remember_created_at
  t.integer  :sign_in_count, default: 0, null: false
  t.datetime :current_sign_in_at
  t.datetime :last_sign_in_at
  t.string   :current_sign_in_ip
  t.string   :last_sign_in_ip
  t.boolean :locked, default: 0
  t.string :name
  t.string :phone, default: ""
  t.string :mobile, default: ""
  t.string :city, default: ""
  t.string :state, default: ""
  t.string :country, default: "Brasil"
  t.string :business, default: ""
  t.boolean :anonymous, default: 0
  t.boolean :admin, default: 0
      
PRIZES:

MESSAGES:
  t.string :name
	t.string :email
	t.string :mobile
	t.string :phone
	t.text :subject
  t.datetime :deleted_at

NEWSLETTERS:
  t.string :email
  
COMMENTS:
  t.string :name
	t.text :texto
	t.string :email
	t.references :place
	t.datetime :deleted_at
	
CATEGORIES:
  t.string :name
	t.string :description
	t.datetime :deleted_at
	t.attachment :photo
	
SUBCATEGORIES:
  t.string :name
	t.references :category
	t.datetime :deleted_at
	
SYSTEM_CONFIGS:
  t.string :email
	t.boolean :systemlocked, default: 0
___________________________________________________________________________________________________________________


