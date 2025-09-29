<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>خانه داری - فروشگاه محصولات خانگی</title>
    <style>
        /* استایل‌های کلی */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Tahoma', Arial, sans-serif;
        }
        
        body {
            background-color: #f9f9f9;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }
        
        /* استایل هدر */
        header {
            background-color: #fff;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .header-top {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
        }
        
        .logo {
            font-size: 24px;
            font-weight: bold;
            color: #4a6fa5;
        }
        
        .search-bar {
            flex-grow: 1;
            max-width: 500px;
            margin: 0 20px;
        }
        
        .search-bar input {
            width: 100%;
            padding: 10px 15px;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        
        .user-actions a {
            margin-right: 15px;
            text-decoration: none;
            color: #555;
        }
        
        nav ul {
            display: flex;
            list-style: none;
            background-color: #4a6fa5;
        }
        
        nav ul li {
            padding: 12px 20px;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
        }
        
        /* استایل اسلایدر */
        .slider {
            height: 400px;
            background-color: #eee;
            margin: 20px 0;
            border-radius: 8px;
            overflow: hidden;
            position: relative;
        }
        
        .slider-content {
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            background: linear-gradient(to right, #4a6fa5, #6b8cc0);
            color: white;
            text-align: center;
            padding: 0 20px;
        }
        
        .slider-content h2 {
            font-size: 32px;
            margin-bottom: 15px;
        }
        
        .slider-content p {
            font-size: 18px;
            margin-bottom: 20px;
        }
        
        .btn {
            display: inline-block;
            background-color: #ff6b6b;
            color: white;
            padding: 10px 20px;
            border-radius: 4px;
            text-decoration: none;
            font-weight: bold;
        }
        
        /* استایل بخش محصولات */
        .section-title {
            text-align: center;
            margin: 30px 0 20px;
            font-size: 24px;
            color: #4a6fa5;
        }
        
        .products {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
            margin-bottom: 40px;
        }
        
        .product-card {
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }
        
        .product-card:hover {
            transform: translateY(-5px);
        }
        
        .product-image {
            height: 200px;
            background-color: #f5f5f5;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .product-info {
            padding: 15px;
        }
        
        .product-title {
            font-weight: bold;
            margin-bottom: 10px;
        }
        
        .product-price {
            color: #ff6b6b;
            font-weight: bold;
            margin-bottom: 10px;
        }
        
        .add-to-cart {
            background-color: #4a6fa5;
            color: white;
            border: none;
            padding: 8px 15px;
            border-radius: 4px;
            cursor: pointer;
            width: 100%;
        }
        
        /* استایل فوتر */
        footer {
            background-color: #333;
            color: white;
            padding: 40px 0 20px;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 30px;
            margin-bottom: 30px;
        }
        
        .footer-column h3 {
            margin-bottom: 15px;
            font-size: 18px;
        }
        
        .footer-column ul {
            list-style: none;
        }
        
        .footer-column ul li {
            margin-bottom: 8px;
        }
        
        .footer-column ul li a {
            color: #ddd;
            text-decoration: none;
        }
        
        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid #555;
        }
        
        /* ریسپانسیو */
        @media (max-width: 768px) {
            .header-top {
                flex-direction: column;
            }
            
            .search-bar {
                margin: 15px 0;
                max-width: 100%;
            }
            
            nav ul {
                flex-wrap: wrap;
            }
            
            .slider {
                height: 300px;
            }
            
            .slider-content h2 {
                font-size: 24px;
            }
            
            .slider-content p {
                font-size: 16px;
            }
        }
    </style>
</head>
<body>
    <!-- هدر سایت -->
    <header>
        <div class="container">
            <div class="header-top">
                <div class="logo">خانه داری</div>
                <div class="search-bar">
                    <input type="text" placeholder="جستجوی محصولات...">
                </div>
                <div class="user-actions">
                    <a href="#">ورود / ثبت‌نام</a>
                    <a href="#">سبد خرید</a>
                </div>
            </div>
            <nav>
                <ul>
                    <li><a href="#">صفحه اصلی</a></li>
                    <li><a href="#">لوازم آشپزخانه</a></li>
                    <li><a href="#">نظافت و بهداشت</a></li>
                    <li><a href="#">دکوراسیون</a></li>
                    <li><a href="#">مشاهده همه</a></li>
                    <li><a href="#">تماس با ما</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- اسلایدر اصلی -->
    <section class="slider">
        <div class="slider-content">
            <div>
                <h2>بهترین محصولات خانگی را از ما بخواهید</h2>
                <p>کیفیت و قیمت مناسب در کنار هم</p>
                <a href="#" class="btn">مشاهده محصولات</a>
            </div>
        </div>
    </section>

    <!-- بخش اصلی محتوا -->
    <main class="container">
        <h2 class="section-title">محصولات پرفروش</h2>
        <div class="products">
            <!-- محصول 1 -->
            <div class="product-card">
                <div class="product-image">تصویر محصول</div>
                <div class="product-info">
                    <div class="product-title">جارو برقی قدرتمند</div>
                    <div class="product-price">۲,۵۰۰,۰۰۰ تومان</div>
                    <button class="add-to-cart">افزودن به سبد خرید</button>
                </div>
            </div>
            
            <!-- محصول 2 -->
            <div class="product-card">
                <div class="product-image">تصویر محصول</div>
                <div class="product-info">
                    <div class="product-title">مخلوط کن چندکاره</div>
                    <div class="product-price">۱,۸۰۰,۰۰۰ تومان</div>
                    <button class="add-to-cart">افزودن به سبد خرید</button>
                </div>
            </div>
            
            <!-- محصول 3 -->
            <div class="product-card">
                <div class="product-image">تصویر محصول</div>
                <div class="product-info">
                    <div class="product-title">مایکروویو دیجیتال</div>
                    <div class="product-price">۳,۲۰۰,۰۰۰ تومان</div>
                    <button class="add-to-cart">افزودن به سبد خرید</button>
                </div>
            </div>
            
            <!-- محصول 4 -->
            <div class="product-card">
                <div class="product-image">تصویر محصول</div>
                <div class="product-info">
                    <div class="product-title">اتو بخار صنعتی</div>
                    <div class="product-price">۱,۵۰۰,۰۰۰ تومان</div>
                    <button class="add-to-cart">افزودن به سبد خرید</button>
                </div>
            </div>
        </div>
        
        <h2 class="section-title">جدیدترین محصولات</h2>
        <div class="products">
            <!-- محصول 5 -->
            <div class="product-card">
                <div class="product-image">تصویر محصول</div>
                <div class="product-info">
                    <div class="product-title">قهوه ساز تمام اتوماتیک</div>
                    <div class="product-price">۴,۵۰۰,۰۰۰ تومان</div>
                    <button class="add-to-cart">افزودن به سبد خرید</button>
                </div>
            </div>
            
            <!-- محصول 6 -->
            <div class="product-card">
                <div class="product-image">تصویر محصول</div>
                <div class="product-info">
                    <div class="product-title">ماشین ظرفشویی</div>
                    <div class="product-price">۱۲,۰۰۰,۰۰۰ تومان</div>
                    <button class="add-to-cart">افزودن به سبد خرید</button>
                </div>
            </div>
            
            <!-- محصول 7 -->
            <div class="product-card">
                <div class="product-image">تصویر محصول</div>
                <div class="product-info">
                    <div class="product-title">پلوپز گازی</div>
                    <div class="product-price">۱,۲۰۰,۰۰۰ تومان</div>
                    <button class="add-to-cart">افزودن به سبد خرید</button>
                </div>
            </div>
            
            <!-- محصول 8 -->
            <div class="product-card">
                <div class="product-image">تصویر محصول</div>
                <div class="product-info">
                    <div class="product-title">سینک ظرفشویی استیل</div>
                    <div class="product-price">۲,۸۰۰,۰۰۰ تومان</div>
                    <button class="add-to-cart">افزودن به سبد خرید</button>
                </div>
            </div>
        </div>
    </main>

    <!-- فوتر سایت -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>دسته‌بندی محصولات</h3>
                    <ul>
                        <li><a href="#">لوازم آشپزخانه</a></li>
                        <li><a href="#">نظافت و بهداشت</a></li>
                        <li><a href="#">دکوراسیون</a></li>
                        <li><a href="#">میز و صندلی</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>خدمات مشتریان</h3>
                    <ul>
                        <li><a href="#">پرسش‌های متداول</a></li>
                        <li><a href="#">رویه بازگرداندن کالا</a></li>
                        <li><a href="#">شرایط استفاده</a></li>
                        <li><a href="#">حریم خصوصی</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>تماس با ما</h3>
                    <ul>
                        <li>تلفن: ۰۲۱-۱۲۳۴۵۶۷۸</li>
                        <li>ایمیل: info@khanehdari.com</li>
                        <li>آدرس: تهران، خیابان ولیعصر</li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>خبرنامه</h3>
                    <p>برای دریافت جدیدترین تخفیف‌ها و محصولات ایمیل خود را وارد کنید</p>
                    <input type="email" placeholder="ایمیل شما" style="padding: 8px; width: 100%; margin-top: 10px;">
                    <button class="btn" style="margin-top: 10px;">عضویت</button>
                </div>
            </div>
            
            <div class="copyright">
                <p>کلیه حقوق این سایت متعلق به فروشگاه خانه داری می‌باشد.</p>
            </div>
        </div>
    </footer>
</body>
</html>
