/* ... (ส่วน nav .container และ logo เหมือนเดิม) ... */

/* MENU UL */
nav .container .menu ul {
    display: flex;
    height: 100%;
    align-items: center;
    list-style: none;
    margin: 0;
    padding: 0;
}

/* MENU LI - ลบระยะห่างระหว่างรายการเมนูออกเพื่อให้ปุ่มชิดกัน */
nav .container .menu ul li {
    margin-left: 0; 
}

/* MENU A - จัดรูปแบบปุ่ม */
nav .container .menu ul li a {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 60px; /* ทำให้ปุ่มสูงเต็ม nav bar (60px) */
    padding: 0 1.5rem; /* กำหนด padding ซ้ายขวาให้ดูเป็นปุ่ม */
    text-decoration: none;
    font-size: 0.9rem;
    font-weight: 600;
    white-space: nowrap; /* ป้องกันข้อความไม่ให้ขึ้นบรรทัดใหม่ */
    /* ลบ border-radius ออก เพื่อให้ปุ่มขอบตรงชิดกัน */
    border-radius: 0; 
    transition: background-color 0.2s;
}

/* MENU A - สไตล์เฉพาะตาม ID */

/* Login: พื้นขาว ขอบดำ */
#l-log {
    background-color: var(--white);
    color: var(--black);
    /* เพิ่มขอบขวา 1px เพื่อแยกกับปุ่ม Donate Now */
    border-right: 1px solid #ccc; 
}
#l-log:hover {
    /* ... */
}

/* Donate Now: ส้ม */
#l-donate {
    background-color: var(--orange);
    color: var(--white);
}

/* Take Action: เหลือง */
#l-take {
    background-color: var(--yellow);
    color: var(--white);
}

/* Menu: ดำ (สามารถเพิ่มไอคอนเมนูใน HTML ได้) */
#l-menu {
    background-color: var(--black);
    color: var(--white);
    /* เพิ่ม padding ด้านขวามากขึ้นเล็กน้อยสำหรับไอคอนเมนู */
    padding-right: 2rem; 
}