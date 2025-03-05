# Qrcode
Qr kodelar yaratish
import qrcode

def generate_qr(data, filename="qr_code.png"):
    qr = qrcode.make(data)
    qr.save(filename)
    print(f"QR kod saqlandi: {filename}")

# Foydalanuvchi matn kiritishi
text = input("QR kod uchun matn yoki URL kiriting: ")
generate_qr(text)
