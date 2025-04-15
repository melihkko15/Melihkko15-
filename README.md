# # E-kitap
window.location.href
import React from "react"; import { Button } from "@/components/ui/button"; import { Card, CardContent } from "@/components/ui/card";

export default function Home() { const handlePurchase = () => { // Geçici test linki (iyzico veya başka bir sağlayıcı ile değiştirilebilir) window.location.href = "https://sandbox-iyzico-payment-page.com"; };

return ( <div className="bg-black text-white min-h-screen p-6"> <header className="text-center text-4xl font-bold mb-8">E-Kitap Dünyası</header>

<section className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
    <Card className="bg-gray-900 text-white rounded-2xl shadow-lg">
      <CardContent className="p-4">
        <h2 className="text-xl font-semibold mb-2">Eşek Ticareti ve Eşeklerle İlgili Her Şey</h2>
        <img 
          src="https://via.placeholder.com/300x200?text=E%C5%9Fek+Kitap" 
          alt="Eşek Kitap Kapağı" 
          className="w-full h-auto mb-4 rounded-lg"
        />
        <p className="mb-4 text-sm">
          Bu e-kitap, eşek bakımı, yetiştiriciliği, ticareti ve daha fazlası hakkında kapsamlı bilgiler sunar.
          Yeni başlayanlardan profesyonellere kadar herkes için değerli bir kaynaktır.
        </p>
        <p className="mb-4 font-bold text-lg">Fiyat: 99 TL</p>
        <Button 
          className="bg-white text-black hover:bg-gray-300 w-full" 
          onClick={handlePurchase}
        >
          Satın Al
        </Button>
      </CardContent>
    </Card>
  </section>

  <footer className="mt-12 text-center text-sm text-gray-400">
    © 2025 E-Kitap Dünyası - Tüm hakları saklıdır.
  </footer>
</div>

); }
