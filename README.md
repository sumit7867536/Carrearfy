# Carrearfy
Carrearfy ek modern career platform hai jo students aur professionals ko career guidance, skills aur growth opportunities provide karta hai.
export default function CarrearfyWebsite() { const services = [ { title: "Career Guidance", desc: "Get personalized career roadmaps, mentorship, and future planning support.", }, { title: "Skill Development", desc: "Learn modern digital, AI, communication, and professional skills.", }, { title: "Job & Exam Support", desc: "Preparation resources, resume building, interview guidance, and exam strategies.", }, ];

const features = [ "Modern responsive design", "Mobile-friendly layout", "Fast loading and SEO-ready", "Clean UI with professional branding", "Easy to expand with blogs, login, or courses", ];

return ( <div className="min-h-screen bg-white text-gray-900"> {/* Navbar */} <header className="sticky top-0 z-50 border-b bg-white/90 backdrop-blur"> <div className="mx-auto flex max-w-7xl items-center justify-between px-6 py-4"> <div> <h1 className="text-2xl font-bold tracking-tight">Carrearfy</h1> <p className="text-sm text-gray-500">Shape Your Future</p> </div>

<nav className="hidden gap-8 md:flex">
        <a href="#services" className="hover:text-black text-gray-600">Services</a>
        <a href="#features" className="hover:text-black text-gray-600">Features</a>
        <a href="#contact" className="hover:text-black text-gray-600">Contact</a>
      </nav>

      <button className="rounded-2xl bg-black px-5 py-2 text-white shadow-lg transition hover:scale-105">
        Get Started
      </button>
    </div>
  </header>

  {/* Hero Section */}
  <section className="relative overflow-hidden">
    <div className="absolute inset-0 bg-gradient-to-br from-gray-100 to-white" />

    <div className="relative mx-auto grid max-w-7xl items-center gap-12 px-6 py-24 md:grid-cols-2">
      <div>
        <div className="mb-4 inline-flex rounded-full border border-gray-300 px-4 py-2 text-sm text-gray-600">
          Career • Skills • Growth
        </div>

        <h2 className="text-5xl font-extrabold leading-tight md:text-6xl">
          Build Your <span className="text-gray-500">Dream Career</span>
        </h2>

        <p className="mt-6 max-w-xl text-lg text-gray-600">
          Carrearfy helps students and professionals discover opportunities,
          improve skills, and achieve career success with modern guidance.
        </p>

        <div className="mt-8 flex flex-wrap gap-4">
          <button className="rounded-2xl bg-black px-6 py-3 text-white shadow-xl transition hover:scale-105">
            Explore Services
          </button>

          <button className="rounded-2xl border border-gray-300 px-6 py-3 transition hover:bg-gray-100">
            Learn More
          </button>
        </div>
      </div>

      <div className="relative">
        <div className="rounded-[32px] border border-gray-200 bg-white p-8 shadow-2xl">
          <div className="space-y-6">
            <div className="rounded-2xl bg-gray-100 p-6">
              <h3 className="text-xl font-semibold">AI Career Assistant</h3>
              <p className="mt-2 text-gray-600">
                Personalized recommendations based on your goals and skills.
              </p>
            </div>

            <div className="grid grid-cols-2 gap-4">
              <div className="rounded-2xl bg-black p-5 text-white">
                <p className="text-3xl font-bold">10K+</p>
                <p className="mt-1 text-sm text-gray-300">Students Guided</p>
              </div>

              <div className="rounded-2xl border border-gray-200 p-5">
                <p className="text-3xl font-bold">95%</p>
                <p className="mt-1 text-sm text-gray-500">Satisfaction</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  {/* Services */}
  <section id="services" className="mx-auto max-w-7xl px-6 py-20">
    <div className="mb-14 text-center">
      <h3 className="text-4xl font-bold">Our Services</h3>
      <p className="mt-4 text-gray-600">
        Everything you need to grow professionally.
      </p>
    </div>

    <div className="grid gap-8 md:grid-cols-3">
      {services.map((service, index) => (
        <div
          key={index}
          className="rounded-3xl border border-gray-200 bg-white p-8 shadow-sm transition hover:-translate-y-2 hover:shadow-xl"
        >
          <h4 className="text-2xl font-semibold">{service.title}</h4>
          <p className="mt-4 leading-relaxed text-gray-600">
            {service.desc}
          </p>
        </div>
      ))}
    </div>
  </section>

  {/* Features */}
  <section id="features" className="bg-gray-50 py-20">
    <div className="mx-auto max-w-6xl px-6">
      <div className="mb-14 text-center">
        <h3 className="text-4xl font-bold">Why Choose Carrearfy?</h3>
        <p className="mt-4 text-gray-600">
          Built for modern learners and professionals.
        </p>
      </div>

      <div className="grid gap-6 md:grid-cols-2">
        {features.map((feature, index) => (
          <div
            key={index}
            className="rounded-2xl border border-gray-200 bg-white p-6 shadow-sm"
          >
            <div className="flex items-center gap-4">
              <div className="flex h-10 w-10 items-center justify-center rounded-full bg-black text-white">
                ✓
              </div>
              <p className="text-lg font-medium">{feature}</p>
            </div>
          </div>
        ))}
      </div>
    </div>
  </section>

  {/* CTA */}
  <section className="px-6 py-24">
    <div className="mx-auto max-w-5xl rounded-[40px] bg-black px-8 py-16 text-center text-white shadow-2xl">
      <h3 className="text-4xl font-bold md:text-5xl">
        Start Building Your Future Today
      </h3>

      <p className="mx-auto mt-6 max-w-2xl text-lg text-gray-300">
        Join Carrearfy and unlock guidance, opportunities, and growth for your career journey.
      </p>

      <button className="mt-10 rounded-2xl bg-white px-8 py-4 text-lg font-semibold text-black transition hover:scale-105">
        Join Now
      </button>
    </div>
  </section>

  {/* Footer */}
  <footer id="contact" className="border-t bg-white">
    <div className="mx-auto grid max-w-7xl gap-12 px-6 py-16 md:grid-cols-3">
      <div>
        <h4 className="text-2xl font-bold">Carrearfy</h4>
        <p className="mt-4 text-gray-600">
          Helping students and professionals create successful careers.
        </p>
      </div>

      <div>
        <h5 className="mb-4 text-lg font-semibold">Quick Links</h5>
        <div className="space-y-3 text-gray-600">
          <p>Home</p>
          <p>Services</p>
          <p>About</p>
          <p>Contact</p>
        </div>
      </div>

      <div>
        <h5 className="mb-4 text-lg font-semibold">Contact</h5>
        <div className="space-y-3 text-gray-600">
          <p>Email: hello@carrearfy.in</p>
          <p>Website: www.carrearfy.in</p>
          <p>India</p>
        </div>
      </div>
    </div>

    <div className="border-t py-6 text-center text-sm text-gray-500">
      © 2026 Carrearfy. All rights reserved.
    </div>
  </footer>
</div>

); }
