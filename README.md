# Mahsollat
Best mahsool
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>کت بانو فاطمه | فروشگاه اینترنتی</title>
    <link rel="stylesheet" href="style.css">
    <!-- لینک فونت ایران سنس -->
    <link rel="stylesheet" href="https://cdn.fontcdn.ir/Font/Persian/IRAN-Sans/IRAN-Sans.css">
</head>
<body>
    <!-- نوار بار بالا -->
    <header class="header">
        <nav class="nav container">
            <a href="#" class="logo">Katbano_Fatemeh</a>
            <ul class="nav-menu">
                <li><a href="#home">خانه</a></li>
                <li><a href="#products">محصولات</a></li>
                <li><a href="#about">درباره ما</a></li>
                <li><a href="#contact">تماس</a></li>
                <li><a href="#" class="login-btn" onclick="openModal('loginModal')">ورود / ثبت نام</a></li>
            </ul>
        </nav>
    </header>

    <!-- بخش اصلی (Hero) -->
    <section id="home" class="hero">
        <div class="hero-content">
            <h1>به دنیای شیک‌پوشی <span>کت بانو فاطمه</span> خوش آمدید</h1>
            <p>مدرن، لوکس و منحصربه‌فرد. بهترین‌ها را از ما بخواهید.</p>
            <a href="#products" class="cta-button">مشاهده محصولات</a>
        </div>
        <div class="hero-overlay"></div>
    </section>

    <!-- بخش محصولات -->
    <section id="products" class="products">
        <div class="container">
            <h2>محصولات منتخب</h2>
            <div class="product-grid">
                <!-- محصول 1 -->
                <div class="product-card">
                    <img src="https://via.placeholder.com/300x400/1E90FF/FFFFFF?text=Product+1" alt="محصول اول">
                    <h3>کت شیک زمستانه</h3>
                    <p>1,290,000 تومان</p>
                    <button class="add-to-cart" onclick="addToCart('کت شیک زمستانه', 1290000)">افزودن به سبد</button>
                </div>
                <!-- محصول 2 -->
                <div class="product-card">
                    <img src="https://via.placeholder.com/300x400/00CED1/FFFFFF?text=Product+2" alt="محصول دوم">
                    <h3>کت مجلسی ابریشمی</h3>
                    <p>1,850,000 تومان</p>
                    <button class="add-to-cart" onclick="addToCart('کت مجلسی ابریشمی', 1850000)">افزودن به سبد</button>
                </div>
                <!-- محصول 3 -->
                <div class="product-card">
                    <img src="https://via.placeholder.com/300x400/FFF5EE/000000?text=Product+3" alt="محصول سوم">
                    <h3>کت اداری کلاسیک</h3>
                    <p>990,000 تومان</p>
                    <button class="add-to-cart" onclick="addToCart('کت اداری کلاسیک', 990000)">افزودن به سبد</button>
                </div>
            </div>
        </div>
    </section>

    <!-- بخش درباره ما -->
    <section id="about" class="about">
        <div class="container">
            <h2>درباره کت بانو فاطمه</h2>
            <p>ما با سال‌ها تجربه در زمینه طراحی و تولید البسه شیک و مدرن، همواره تلاش کرده‌ایم تا بهترین کیفیت و طراحی‌ها را به مشتریان خود ارائه دهیم. اعتماد شما، سرمایه ماست.</p>
        </div>
    </section>

    <!-- بخش تماس با ما -->
    <section id="contact" class="contact">
        <div class="container">
            <h2>راه های ارتباطی برای خرید</h2>
            <div class="contact-info">
                <p>برای سفارش و مشاوره، از طریق راه‌های زیر با ما در ارتباط باشید:</p>
                <a href="tel:+989104114821" class="phone-link">📞 09104114821</a>
                <p>این شماره در واتس‌اپ و تلگرام نیز فعال است.</p>
            </div>
            <form class="contact-form">
                <input type="text" placeholder="نام شما" required>
                <input type="email" placeholder="ایمیل شما" required>
                <textarea placeholder="پیام شما..." rows="5" required></textarea>
                <button type="submit">ارسال پیام</button>
            </form>
        </div>
    </section>

    <!-- فوتر -->
    <footer class="footer">
        <div class="container">
            <p>© 2023 Katbano_Fatemeh.com - تمام حقوق محفوظ است.</p>
        </div>
    </footer>

    <!-- مودال ورود/ثبت نام -->
    <div id="loginModal" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeModal('loginModal')">&times;</span>
            <h2>ورود / ثبت نام</h2>
            <form id="authForm">
                <input type="email" id="email" placeholder="ایمیل خود را وارد کنید" required>
                <input type="password" id="password" placeholder="رمز عبور" required>
                <button type="submit">ورود</button>
            </form>
            <p>اگر حساب کاربری ندارید، با وارد کردن ایمیل و رمز عبور، حساب جدید ساخته می‌شود.</p>
        </div>
    </div>

    <!-- سبد خرید -->
    <div id="cartSidebar" class="cart-sidebar">
        <div class="cart-header">
            <h3>سبد خرید شما</h3>
            <span class="close-cart" onclick="closeCart()">&times;</span>
        </div>
        <div class="cart-items">
            <!-- آیتم های سبد خرید اینجا نمایش داده می شوند -->
        </div>
        <div class="cart-total">
            <p>جمع کل: <span id="totalPrice">0</span> تومان</p>
            <button class="checkout-btn" onclick="checkout()">تکمیل فرآیند خرید</button>
        </div>
    </div>

    <!-- آیکون سبد خرید -->
    <div class="cart-icon" onclick="openCart()">
        🛒 <span id="cartCount">0</span>
    </div>

    <script src="script.js"></script>
</body>
</html>
/* Reset و فونت */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'IRAN Sans', sans-serif;
}

body {
    background-color: #000000;
    color: #FFFFFF;
    line-height: 1.6;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* هدر و نویگیشن */
.header {
    background-color: rgba(13, 13, 13, 0.95);
    padding: 1rem 0;
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 1000;
    backdrop-filter: blur(10px);
}

.nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 1.5rem;
    font-weight: bold;
    color: #00CED1; /* آبی فیروزه ای */
    text-decoration: none;
}

.nav-menu {
    display: flex;
    list-style: none;
    gap: 2rem;
}

.nav-menu a {
    color: #FFFFFF;
    text-decoration: none;
    transition: color 0.3s ease;
}

.nav-menu a:hover {
    color: #00CED1;
}

.login-btn {
    background: linear-gradient(45deg, #00CED1, #1E90FF);
    padding: 0.5rem 1rem;
    border-radius: 5px;
    color: #000 !important;
    font-weight: bold;
}

/* بخش هیرو */
.hero {
    height: 100vh;
    background: 
        linear-gradient(45deg, rgba(0, 0, 0, 0.8), rgba(255, 245, 238, 0.2)),
        url('https://via.placeholder.com/1920x1080/000000/FFFFFF?text=Black+Luxury+Background');
    background-size: cover;
    background-position: center;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    position: relative;
}

.hero-content h1 {
    font-size: 3rem;
    margin-bottom: 1rem;
}

.hero-content h1 span {
    color: #00CED1;
}

.hero-content p {
    font-size: 1.2rem;
    margin-bottom: 2rem;
    color: #FFF5EE; /* سفید صدفی */
}

.cta-button {
    background: linear-gradient(45deg, #1E90FF, #00CED1);
    color: #000;
    padding: 1rem 2rem;
    text-decoration: none;
    border-radius: 5px;
    font-weight: bold;
    transition: transform 0.3s ease;
}

.cta-button:hover {
    transform: translateY(-3px);
}

/* بخش محصولات */
.products {
    padding: 5rem 0;
    background: linear-gradient(to bottom, #000000, #0D0D0D);
}

.products h2 {
    text-align: center;
    margin-bottom: 3rem;
    font-size: 2.5rem;
    color: #FFF5EE;
}

.product-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 2rem;
}

.product-card {
    background: rgba(255, 255, 255, 0.05);
    border-radius: 10px;
    padding: 1.5rem;
    text-align: center;
    backdrop-filter: blur(10px);
    border: 1px solid rgba(255, 245, 238, 0.1);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.product-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 10px 30px rgba(30, 144, 255, 0.3);
}

.product-card img {
    width: 100%;
    border-radius: 5px;
    margin-bottom: 1rem;
}

.product-card h3 {
    margin-bottom: 0.5rem;
    color: #FFF5EE;
}

.product-card p {
    font-weight: bold;
    color: #00CED1;
    margin-bottom: 1rem;
}

.add-to-cart {
    background: linear-gradient(45deg, #00CED1, #1E90FF);
    color: #000;
    border: none;
    padding: 0.75rem 1.5rem;
    border-radius: 5px;
    cursor: pointer;
    font-weight: bold;
    transition: all 0.3s ease;
    width: 100%;
}

.add-to-cart:hover {
    background: linear-gradient(45deg, #1E90FF, #00CED1);
}

/* بخش درباره ما */
.about {
    padding: 5rem 0;
    background: linear-gradient(45deg, rgba(255, 245, 238, 0.1), rgba(0, 0, 0, 0.9));
    text-align: center;
}

.about h2 {
    margin-bottom: 2rem;
    font-size: 2.5rem;
    color: #FFF5EE;
}

.about p {
    max-width: 800px;
    margin: 0 auto;
    font-size: 1.1rem;
    line-height: 1.8;
}

/* بخش تماس */
.contact {
    padding: 5rem 0;
    background: linear-gradient(to bottom, #0D0D0D, #000000);
}

.contact h2 {
    text-align: center;
    margin-bottom: 3rem;
    font-size: 2.5rem;
    color: #FFF5EE;
}

.contact-info {
    text-align: center;
    margin-bottom: 3rem;
}

.phone-link {
    display: inline-block;
    background: linear-gradient(45deg, #00CED1, #1E90FF);
    color: #000;
    padding: 1rem 2rem;
    border-radius: 5px;
    text-decoration: none;
    font-weight: bold;
    margin: 1rem 0;
    font-size: 1.2rem;
}

.contact-form {
    max-width: 600px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    gap: 1rem;
}

.contact-form input,
.contact-form textarea {
    padding: 1rem;
    border: 1px solid rgba(255, 245, 238, 0.2);
    border-radius: 5px;
    background: rgba(255, 255, 255, 0.05);
    color: #FFF;
    backdrop-filter: blur(10px);
}

.contact-form button {
    background: linear-gradient(45deg, #1E90FF, #00CED1);
    color: #000;
    border: none;
    padding: 1rem;
    border-radius: 5px;
    cursor: pointer;
    font-weight: bold;
    transition: all 0.3s ease;
}

.contact-form button:hover {
    background: linear-gradient(45deg, #00CED1, #1E90FF);
}

/* فوتر */
.footer {
    background: #0D0D0D;
    padding: 2rem 0;
    text-align: center;
    border-top: 1px solid rgba(255, 245, 238, 0.1);
}

/* مودال */
.modal {
    display: none;
    position: fixed;
    z-index: 2000;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.8);
    backdrop-filter: blur(5px);
}

.modal-content {
    background: linear-gradient(45deg, #0D0D0D, #000);
    margin: 10% auto;
    padding: 2rem;
    border-radius: 10px;
    width: 90%;
    max-width: 400px;
    border: 1px solid rgba(255, 245, 238, 0.2);
    position: relative;
}

.close {
    color: #FFF;
    float: left;
    font-size: 2rem;
    font-weight: bold;
    cursor: pointer;
}

.modal h2 {
    margin-bottom: 1.5rem;
    text-align: center;
    color: #FFF5EE;
}

.modal input {
    width: 100%;
    padding: 1rem;
    margin-bottom: 1rem;
    border: 1px solid rgba(255, 245, 238, 0.2);
    border-radius: 5px;
    background: rgba(255, 255, 255, 0.05);
    color: #FFF;
}

.modal button {
    width: 100%;
    padding: 1rem;
    background: linear-gradient(45deg, #00CED1, #1E90FF);
    color: #000;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-weight: bold;
}

/* سبد خرید */
.cart-icon {
    position: fixed;
    bottom: 2rem;
    left: 2rem;
    background: linear-gradient(45deg, #00CED1, #1E90FF);
    color: #000;
    padding: 1rem;
    border-radius: 50%;
    cursor: pointer;
    font-size: 1.5rem;
    z-index: 1000;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
    width: 70px;
    height: 70px;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
}

.cart-sidebar {
    position: fixed;
    top: 0;
    left: -400px;
    width: 350px;
    height: 100%;
    background: linear-gradient(45deg, #0D0D0D, #000);
    box-shadow: -5px 0 15px rgba(0, 0, 0, 0.5);
    transition: left 0.3s ease;
    z-index: 1500;
    padding: 1rem;
    border-left: 1px solid rgba(255, 245, 238, 0.2);
}

.cart-sidebar.active {
    left: 0;
}

.cart-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 2rem;
    padding-bottom: 1rem;
    border-bottom: 1px solid rgba(255, 245, 238, 0.2);
}

.close-cart {
    font-size: 2rem;
    cursor: pointer;
    color: #FFF;
}

.cart-item {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 0;
    border-bottom: 1px solid rgba(255, 245, 238, 0.1);
}

.checkout-btn {
    width: 100%;
    padding: 1rem;
    background: linear-gradient(45deg, #00CED1, #1E90FF);
    color: #000;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-weight: bold;
    margin-top: 1rem;
}

/* رسپانسیو */
@media (max-width: 768px) {
    .nav-menu {
        display: none;
    }
    
    .hero-content h1 {
        font-size: 2rem;
    }
    
    .product-grid {
        grid-template-columns: 1fr;
    }
    
    .cart-sidebar {
        width: 300px;
    }
    
    .cart-icon {
        bottom: 1rem;
        left: 1rem;
    }
}
// مدیریت سبد خرید
let cart = [];
let totalPrice = 0;

function addToCart(productName, productPrice) {
    cart.push({ name: productName, price: productPrice });
    updateCart();
    showNotification(`"${productName}" به سبد خرید اضافه شد!`);
}

function updateCart() {
    const cartCount = document.getElementById('cartCount');
    const cartItems = document.querySelector('.cart-items');
    const totalPriceElement = document.getElementById('totalPrice');
    
    // آپدیت تعداد
    cartCount.textContent = cart.length;
    
    // آپدیت آیتم‌ها
    cartItems.innerHTML = '';
    totalPrice = 0;
    
    cart.forEach(item => {
        totalPrice += item.price;
        const cartItem = document.createElement('div');
        cartItem.className = 'cart-item';
        cartItem.innerHTML = `
            <span>${item.name}</span>
            <span>${item.price.toLocaleString()} تومان</span>
        `;
        cartItems.appendChild(cartItem);
    });
    
    // آپدیت جمع کل
    totalPriceElement.textContent = totalPrice.toLocaleString();
}

function openCart() {
    document.getElementById('cartSidebar').classList.add('active');
}

function closeCart() {
    document.getElementById('cartSidebar').classList.remove('active');
}

function checkout() {
    if (cart.length === 0) {
        alert('سبد خرید شما خالی است!');
        return;
    }
    
    const message = `سفارش جدید از katbano_fatemeh.com:\n\n${cart.map(item => 
        `📦 ${item.name} - ${item.price.toLocaleString()} تومان`
    ).join('\n')}\n\n💰 جمع کل: ${totalPrice.toLocaleString()} تومان`;
    
    // ارسال به واتساپ
    const phone = "989104114821";
    const url = `https://wa.me/${phone}?text=${encodeURIComponent(message)}`;
    window.open(url, '_blank');
    
    // خالی کردن سبد خرید
    cart = [];
    updateCart();
    closeCart();
}

// مدیریت مودال
function openModal(modalId) {
    document.getElementById(modalId).style.display = 'block';
}

function closeModal(modalId) {
    document.getElementById(modalId).style.display = 'none';
}

// مدیریت فرم ورود
document.getElementById('authForm').addEventListener('submit', function(e) {
    e.preventDefault();
    const email = document.getElementById('email').value;
    const password = document.getElementById('password').value;
    
    // اینجا می‌توانید درخواست AJAX به سرور بفرستید
    alert(`با ایمیل: ${email} وارد شدید! (این یک نمونه است)`);
    closeModal('loginModal');
});

// نوتیفیکیشن
function showNotification(message) {
    const notification = document.createElement('div');
    notification.style.cssText = `
        position: fixed;
        top: 100px;
        right: 20px;
        background: linear-gradient(45deg, #00CED1, #1E90FF);
        color: #000;
        padding: 1rem 2rem;
        border-radius: 5px;
        z-index: 3000;
        font-weight: bold;
        animation: slideIn 0.3s ease;
    `;
    notification.textContent = message;
    document.body.appendChild(notification);
    
    setTimeout(() => {
        notification.remove();
    }, 3000);
}

// بستن مودال با کلیک خارج از آن
window.onclick = function(event) {
    const modals = document.getElementsByClassName('modal');
    for (let modal of modals) {
        if (event.target === modal) {
            modal.style.display = 'none';
        }
    }
}

// اسکرول نرم
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
        e.preventDefault();
        const target = document.querySelector(this.getAttribute('href'));
        if (target) {
            target.scrollIntoView({
                behavior: 'smooth',
                block: 'start'
            });
        }
    });
});

// افزودن استایل انیمیشن برای نوتیفیکیشن
const style = document.createElement('style');
style.textContent = `
    @keyframes slideIn {
        from { transform: translateX(100%); opacity: 0; }
        to { transform: translateX(0); opacity: 1; }
    }
`;
document.head.appendChild(style);


