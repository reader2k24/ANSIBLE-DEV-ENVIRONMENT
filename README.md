<h1>Клонирование репозитория</h1>
<pre><code>git clone https://github.com/reader2k24/ANSIBLE-DEV-ENVIRONMENT.git</code></pre>

<h1>Настройка среды разработки с помощью Ansible</h1>
<p>Этот Ansible playbook автоматизирует настройку среды разработки для различных технологий, включая Angular, Docker, PostgreSQL, Redis, Django, Flask и Visual Studio Code. Он устанавливает необходимые зависимости и настраивает среду для беспрепятственной разработки.</p>

<h2>Структура плейбука</h2>
<ol>
  <li>Настройка Docker: Устанавливает Docker и Docker-Compose.</li>
  <li>Установка Docker (PIP): Устанавливает Docker с использованием Python pip.</li>
  <li>Управление пользователями: Добавляет текущего пользователя в группу Docker и выполняет перезагрузку сервера.</li>
  <li>Настройка Angular: Устанавливает NodeJS, Npm и Angular CLI.</li>
  <li>Установка PostgreSQL и Redis: Устанавливает серверы PostgreSQL и Redis.</li>
  <li>Настройка Django и Flask: Создает виртуальное окружение Python и устанавливает необходимые пакеты.</li>
  <li>Настройка Visual Studio Code: Устанавливает Microsoft Visual Studio Code.</li>
</ol>

<h2>Использование</h2>
<ol>
  <li>Клонируйте репозиторий на локальную машину.</li>
  <li>Измените файл hosts, чтобы указать IP-адреса или имена хостов ваших целевых серверов.</li>
  <li>Настройте переменные в каталоге vars в соответствии с вашими требованиями.</li>
  <li>Запустите плейбук с помощью следующей команды:<br><code>ansible-playbook -i inventory all.yml</code></li>
</ol>
<p>Убедитесь, что на вашей локальной машине установлен Ansible перед запуском плейбука.</p>

<h2>Предварительные требования</h2>
<ul>
  <li>Установленный Ansible на локальной машине.</li>
  <li>Целевые серверы доступны по SSH с привилегиями sudo.</li>
</ul>
