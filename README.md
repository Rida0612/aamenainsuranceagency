# aamenainsuranceagency
import React from "react";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";
import { PhoneCall, Home, Car, Building2, Truck } from "lucide-react";

export default function HomePage() {
return (
<div className="min-h-screen bg-white text-gray-800">
 {/* Hero Section */}
 <section className="bg-blue-900 text-white p-10 text-center">
 <h1 className="text-4xl font-bold mb-2">Protect What Matters Most</h1>
 <p className="text-xl mb-6">
  Auto, Home & Commercial Insurance You Can Trust
  </p>
   <div className="flex justify-center gap-4">
   <Button className="bg-white text-blue-900 font-bold">Request a Free Quote</Button>
   <Button className="bg-yellow-400 text-blue-900 font-bold">
   <PhoneCall className="mr-2" /> Call to Enquire
   </Button>
   </div>
   </section>
     
   {/* Services Section */}
    <section className="p-10 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
    <Card>
    <CardContent className="p-4 flex flex-col items-center">
    <Car className="w-10 h-10 mb-2 text-blue-700" />
     <h3 className="font-bold mb-1">Auto Insurance</h3>
     <p className="text-sm text-center">Coverage for accidents, theft & more</p>
     </CardContent>
     </Card>
     <Card>
     <CardContent className="p-4 flex flex-col items-center">
       <Building2 className="w-10 h-10 mb-2 text-blue-700" />
            <h3 className="font-bold mb-1">Business Insurance</h3>
            <p className="text-sm text-center">Keep your business safe & compliant</p>
          </CardContent>
        </Card>
        <Card>
          <CardContent className="p-4 flex flex-col items-center">
            <Truck className="w-10 h-10 mb-2 text-blue-700" />
            <h3 className="font-bold mb-1">Commercial Auto</h3>
            <p className="text-sm text-center">Secure your commercial vehicles</p>
          </CardContent>
        </Card>
      </section>

      {/* Call to Enquire Section */}
      <section className="bg-yellow-100 p-10 text-center">
        <h2 className="text-2xl font-bold mb-2">Got Questions? We’re Just a Call Away!</h2>
        <p className="mb-4">Our agents are ready to help you find the right coverage.</p>
        <Button className="bg-blue-900 text-white font-bold text-lg">
          <PhoneCall className="mr-2" /> Call Now: (123) 456-7890
        </Button>
      </section>

      {/* Testimonials Section */}
      <section className="p-10 bg-gray-50">
        <h2 className="text-center text-2xl font-bold mb-6">What Our Clients Say</h2>
        <div className="grid md:grid-cols-2 gap-6">
          <Card>
            <CardContent className="p-4">
              <p className="italic">
                "Aamena Insurance helped me lower my car insurance and explained everything clearly. Highly recommend!"
              </p>
              <p className="mt-2 font-bold">— Sarah M., Chicago, IL</p>
            </CardContent>
          </Card>
          <Card>
            <CardContent className="p-4">
              <p className="italic">
                "They made getting business insurance for my small shop so easy."
              </p>
              <p className="mt-2 font-bold">— Ahmed R., Naperville, IL</p>
            </CardContent>
          </Card>
        </div>
      </section>
    </div>
  );
}
