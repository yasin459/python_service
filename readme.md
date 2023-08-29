## نحوه راه اندازی:

تنها کافیست که دستور زیر را در  root  اجرا کنید:

docker-compose up --build --scale master=2

### ابتدا با اسکرین شات به درخواست ها پاسخ میدهیم:

####   نمودار UML
![image](https://github.com/yasin459/python_service/assets/60640286/60bb2289-4785-476c-9e73-b39c619fff74)

###  فایل های docker را در مخزن مشاهده میکنید.

#### نتیجه اجرای دستورات بیلد 
![image](https://github.com/yasin459/python_service/assets/60640286/29c941fe-b0ef-4f56-9fd2-2ee61e018d39)

![image](https://github.com/yasin459/python_service/assets/60640286/f9d2c1c6-7bc3-4707-b872-28508d8204d5)

![image](https://github.com/yasin459/python_service/assets/60640286/974c3433-4631-46bc-8b0a-7d932b7d226d)

![image](https://github.com/yasin459/python_service/assets/60640286/a35a4b34-72ff-41fc-9554-4cdf31b27434)


####  دستورات  docker ps , docker images
![image](https://github.com/yasin459/python_service/assets/60640286/f77372b0-1049-446a-81bf-c4bcb326f7d0)


#### تست گرفتن:
 دسترسی به هواشناسی به کمک پورت 100 enginx
![image](https://github.com/yasin459/python_service/assets/60640286/ab32e530-98b4-466f-81cf-966289aef0c3)

دسترسی به اخبار به کمک پورت ۱۰۰  enginx
![image](https://github.com/yasin459/python_service/assets/60640286/f1f3bd01-eb13-4597-8416-80a133e7a5a6)

نمونه ای از  load balancing  به کمک  round robin: همه ی دستورات به نوبت و یکی یکی بین نود های مستر پخش میشوند:

![image](https://github.com/yasin459/python_service/assets/60640286/2b48a78d-b1c0-4920-8194-99b7fe234827)

![image](https://github.com/yasin459/python_service/assets/60640286/b96479b5-c3f1-48fc-b032-1cc1daaf6aa8)


### سوالات

۱. معمولا از نمودار  object و یا نمودار  block  برای نمایش مایکرو سرویس ها استفاده میشود.

۲. در واقع Domain-driven Design (DDD) و معماری Microservice دو مفهوم مرتبط در زمینه توسعه نرم‌افزار هستند. DDD به ما کمک می‌کند تا با تمرکز بر روی دامنه‌ی کسب‌وکار، مدل‌های غنی و هماهنگ با زبان کسب‌وکار را ایجاد کنیم. این مدل‌ها به عنوان مرکز برای طراحی و پیاده‌سازی سرویس‌های میکروسرویس عمل می‌کنند. معماری Microservice، سیستم بزرگ را به سرویس‌های کوچک‌تر و مستقل تقسیم می‌کند که هر کدام به عنوان یک سرویس جداگانه عمل می‌کنند و با استفاده از مفاهیم DDD، هر سرویس میکروسرویس می‌تواند دامنه‌ی کسب‌وکار خود را با مدل‌های غنی و هماهنگ توسعه دهد.

۳. باید توجه کنیم که Docker Compose نه تنها یک ابزار Orchestration نیست، بلکه یک ابزار مدیریت و اجرای برنامه‌های چند سرویسی در Docker است. Docker Compose اجازه می‌دهد تا برنامه‌های ساخته شده از چندین سرویس Docker را به صورت مشترک و به هماهنگی با یکدیگر اجرا کند و تنظیمات مربوط به شبکه‌ها، ذخیره‌سازی داده و پارامترهای محیطی را مدیریت کند. در اصل، Docker Compose کمک می‌کند تا به راحتی برنامه‌های چند سرویسی در Docker را مدیریت و اجرا کنیم.





