---
title: '9.4 الگوهای همزمانی'
weight: 17700
bookCollapseSection: true
---


| عنوان  | توضیحات | وضعیت | 
|---|----------|-------------|
| [Wait For Result](../../chapter-9/concurrency-patterns/go-concurrency-pattern-wait-for-result) | با استفاده از الگو Wait For Result می توانید یک عملیاتی را بصورت همزمانی انجام دهید و سپس منتظر نتیجه عملیات صورت گرفته بمانید. برای اینکار از کانال استفاده می شود. | ✅     |
| [Fan Out/In](../../chapter-9/concurrency-patterns/go-concurrency-pattern-fan-out-in) | الگو Fan Out/In یک تکنیک همزمانی در زبان گو می باشد که به شما اجازه می دهد چندین کار را با گوروتین همزمان انجام دهید و در نتیجه خروجی این کارها را با هم ترکیب کنید و به عنوان نتیجه نهایی دریافت کنید.    | ✅     |
| [Wait For Task](../../chapter-9/concurrency-patterns/go-concurrency-pattern-wait-for-task) | الگو wait for task یکی از الگوهای رایج در زبان گو می باشد و انتظار برای تکمیل یک تسک یا فرآیند استفاده می شود. یک تسک با استفاده از گوروتین اجرا می شود و پس اتمامش کار تسک از طریق کانال سیگنال انجام می فرستد.    | ✅     |
| [Drop](../../chapter-9/concurrency-patterns/go-concurrency-pattern-drop) | الگو Drop یک الگو مهم برای انجام خدمات سنگین می باشد. خدماتی که مواقعی باعث می شود حجم درخواست هایش بیش از ظرفیت موجود باشد و این درخواست ها بواسطه این الگو می تواند Drop شود. به عنوان مثال سرویس های DNS باید از این الگو استفاده کنند.    | ✅     |
| [Cancellation](../../chapter-9/concurrency-patterns/go-concurrency-pattern-cancellation) | الگو cancellation که حرکت تکنیکی هست برای ارسال سینگال به گوروتین ها استفاده می شود که باید اجرای کاری را متوقف کند و ایده اصلی این کار با استفاده بستن کانال صورت میگیرد.    | ✅     |
| [Semaphore](../../chapter-9/concurrency-patterns/go-concurrency-pattern-semaphore) | الگو Semaphore برای مدیریت کنترل دسترسی به منابع مشترک در همزمانی استفاده می شود. فرض کنید بصورت موازی ۱۰۰ درخواست HTTP سمت سرور میاد و I/O شبکه برای پردازش همزمان این ۱۰۰ درخواست درگیر میشود و به مرور عملکرد کاهش می یابد. حال اگر ما بیایم این ۱۰۰ درخواست موازی را تقسیم کنیم به ۵ دسته ۲۰ تایی که بصورت همزمانی انجام شود باعث می شود I/O شبکه کاهش یابد و عملکرد بهتری را خواهیم داشت.    | ✅     |
| [Bounded Work Pooling](../../chapter-9/concurrency-patterns/go-concurrency-pattern-bounded-work-pooling) | با استفاده از الگو Bounded Work Pooling  امکان محدود سازی تعداد گوروتین ها را براساس کار مشخصی دارید و گوروتین ها را محدود به تعداد دفعات کار مشخص شده محدود می شود. این الگو برای وقت مفید است که شما می خواهید منابع را به یک کار خاص محدود کنید.    | ✅     |
| [Retry Timeout](../../chapter-9/concurrency-patterns/go-concurrency-pattern-retry-timeout) | شما از الگو Retry Timeout برای تلاش مجدد یکسری عملیات استفاده کنید. برای اینکار شما می توانید از حلقه و تابع After در پکیج time کمک بگیرید و برای هرتلاش یک timeout مشخص کنید.    | ✅     |
| [Channel Cancellation](../../chapter-9/concurrency-patterns/go-concurrency-pattern-channel-cancellation) | از کانال ها برای ارتباط بین گوروتین ها و هماهنگ کردن اجرا استفاده می شود. حال گاهی اوقات نیاز است که ما یکسری فرآیند را داخل گوروتین لغو کنیم. در اینجا می توانیم با استفاده از کانال سیگنال لغو کردن بفرستید تا عملیات هایی که گوروتین مورد نظر انجام می داد لغو شود.    | ✅     |
| [Producer-Consumer](../../chapter-9/concurrency-patterns/go-concurrency-pattern-producer-consumer) | الگو producer-consumer یکی از کاربردی ترین الگوها در زبان گو می باشد که با استفاده از الگو می توانید بطور همزمان یکسری اطلاعات تولید کنید و بفرستید داخل کانال و این اطلاعات توسط مصرف کننده بواسطه کانال دریافت شود.    | ✅     |
| [Monitor](../../chapter-9/concurrency-patterns/go-concurrency-pattern-monitor) | الگوی مانیتور به گروتین‌ ها اجازه می‌دهد هنگام ورود به حالت خواب بدون مسدود کردن اجرا یا مصرف منابع، منتظر شرایط خاصی باشند.    | ✅     |
| [Future](../../chapter-9/concurrency-patterns/go-concurrency-pattern-future) | در زبان گو الگو Future راهی برای نمایش نتیجه یک عملیات ناهمزمان (asynchronous) است که ممکن است آن عملیات هنوز تکمیل نشده باشد اما این الگو به شما این امکان را می دهد کدی بنویسید که طوری رفتار کند که گویی نتیجه یک عملیات فورا در دسترس است. حتی اگر عملیات در پس زمینه در حال اجرا باشد.    | ✅     |
| [Pipeline](../../chapter-9/concurrency-patterns/go-concurrency-pattern-pipeline) | الگو خط لوله (Pipeline) یکی از پرکاربردی ترین الگوها در همزمانی می باشد شما با استفاده از این الگو می توانید تسک های بزرگ را به تسک های کوچکتر و مستقل تقسیم کنید که می توانند بطور همزمان کار کنند. هر stage داخل یک گوروتین انجام می شود و بواسطه کانال داده ها بین stage های مختلف منتقل می شود.    | ✅     |
| [Subscription](../../chapter-9/concurrency-patterns/go-concurrency-pattern-subscription) | الگو Subscription یکی از الگوهای کاربردی برای پیاده سازی consumer می باشد که به یک آدرسی مشترک شوید و در بازده زمانی مختلف درخواست دهید و یکسری اطلاعات دریافت کنید.    | ✅     |
| [Bridge Channel](../../chapter-9/concurrency-patterns/go-concurrency-pattern-brdige-channel) | با استفاده از الگو Bridge Channel می توانید بین ۲ کانال داده ای را منتقل کنید فرض کنید یک داده را به کانال input میفرستید و از دریافت داده آن را می توانید به کانال دیگری منتقل کنید و عملا شما یک پل برای انتقال داده ایجاد کردید.    | ✅     |
| [Queuing](../../chapter-9/concurrency-patterns/go-concurrency-pattern-queuing) | الگوی "صف" در زبان گو الگویی است که در آن از یک گوروتین برای بافر کردن و مدیریت ترتیب مقادیر ارسال شده و دریافت شده از یک کانال استفاده می شود.    | ✅     |