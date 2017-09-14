#Starting your social website project
<ul>
  <li>mkdir env</li>
  <li>virtualenv env/bookmarks</li>
  <li>source env/bookmarks/bin/activate</li>
  <li>django-admin startproject bookmarks</li>
  <li>cd bookmarks</li>
  <li>django-admin startapp account</li>
</ul>

To activate the new application in your project by adding it to the INSTALLED_APPS setting in the settings.py. 
Then command:
<ul>
  <li>python manage.py migrate</li>
</ul>

+AuthenticationMiddleware: Kết hợp users với request sử dụng session
+SessionMiddleware: Sử lý session hiện tại thông qua requests.
- Authentication framework bao gồm các models sau:
<ul>
  <li>user: Một user gồm các trường cơ bản sau: username, password, email, first_name, last_name, is_active.</li> 
  <li>Group: Một model group để phân nhóm users.</li>
  <li>Permission: Flags để thực hiện một hành động nhất định</li>
</ul>

- Tạo 1 log-in view có các yêu cầu sau:
<ul>
  <li>Lấy thông tin username và password tại form.</li>
  <li>Xác thực xem user có được lưu trữ trong database không.</li>
  <li>Kiểm tra user có hoạt động không</li>
  <li>Log user vào website và bắt đầu xác thực session.</li>
</ul>


