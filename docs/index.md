from selenium import webdriver
from selenium.webdriver.common.keys import Keys
import pyperclip

# O link da sua plataforma
link = "https://pa3333.com/?invite_code=HLQYSWOJ

# Copiando o link para a área de transferência
pyperclip.copy(link)

# Configurando o WebDriver (supondo que você esteja usando o Chrome)
driver = webdriver.Chrome(executable_path="/caminho/para/chromedriver")

# Abrindo a página onde você quer colar o link
driver.get("https://pa3333.com/?invite_code=HLQYSWOJ")

# Encontrando o campo de texto onde você quer colar o link (exemplo de busca por nome do campo)
campo_texto = driver.find_element_by_name("nome_do_campo")

# Colando o link no campo de texto
campo_texto.send_keys(Keys.CONTROL, 'v')

# Opcional: Submeter o formulário
# campo_texto.submit()


