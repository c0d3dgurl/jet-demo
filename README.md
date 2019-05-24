# Demo for Django JET

## 操作步骤
```bash
mkdir jet-demo
cd jet-demo
django-admin startproject main .
pip install django-jet
# TODO: Fllow https://github.com/geex-arts/django-jet/blob/dev/README.rst#installation
# 修改settings.py中 INSTALLED_APPS, 调整 "admin" 到 "jet" 之后
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver 127.0.0.1:9090
# visit by: http://127.0.0.1:9090/admin/
```

## 自定义菜单
使用命令 `python manage.py jet_side_menu_items_example` 获取现有菜单，然后修改依据此修改 `settings.py` 中 `JET_SIDE_MENU_ITEMS`

## Bug处理
* [Unable to add widget #284](https://github.com/geex-arts/django-jet/issues/284#issuecomment-359195347)

## 说明
* `!overwrite!`为重写内容(模板等)目录
