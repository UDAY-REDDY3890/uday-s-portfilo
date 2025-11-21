import { Button } from "@/components/ui/button";
import { Card } from "@/components/ui/card";
import { Download, Mail, Linkedin, Github, Server, Cloud, Container, Terminal, Code2, Cpu } from "lucide-react";

const Index = () => {
  const skills = [
    "Linux", "Shell Scripting", "Git & GitHub", "CI/CD", "Docker", 
    "Nginx", "Automation", "AWS", "Python", "Java"
  ];

  const timeline = [
    { year: "2024", event: "Started DevOps Journey" },
    { year: "2024", event: "Linux & Shell Scripting" },
    { year: "2025", event: "AWS & Cloud Fundamentals" },
    { year: "2025", event: "Docker & Containerization" },
    { year: "2025", event: "Built Nginx Reverse Proxy Project" },
    { year: "2025", event: "Portfolio Website" },
  ];

  return (
    <div className="min-h-screen bg-background text-foreground overflow-x-hidden relative">
      {/* Animated Cloud Background */}
      <div className="fixed inset-0 overflow-hidden pointer-events-none z-0">
        <div className="cloud w-96 h-96 top-20 left-[-10%]" style={{ animationDelay: "0s", animationDuration: "70s" }} />
        <div className="cloud w-[500px] h-[500px] top-40 right-[-15%]" style={{ animationDelay: "10s", animationDuration: "90s" }} />
        <div className="cloud w-80 h-80 bottom-40 left-[-5%]" style={{ animationDelay: "20s", animationDuration: "80s" }} />
        <div className="cloud w-[600px] h-[600px] top-60 left-[30%]" style={{ animationDelay: "30s", animationDuration: "100s" }} />
        <div className="cloud w-[450px] h-[450px] bottom-20 right-[-10%]" style={{ animationDelay: "15s", animationDuration: "85s" }} />
      </div>

      {/* Hero Section */}
      <section className="relative min-h-screen flex items-center justify-center px-4 py-20 z-10">
        {/* Animated Background Grid */}
        <div className="absolute inset-0 bg-[linear-gradient(to_right,#00ffff0a_1px,transparent_1px),linear-gradient(to_bottom,#00ffff0a_1px,transparent_1px)] bg-[size:4rem_4rem]" />
        
        {/* Floating DevOps Icons */}
        <div className="absolute inset-0 overflow-hidden pointer-events-none">
          <Server className="absolute top-20 left-[10%] w-12 h-12 text-primary/30 floating" style={{ animationDelay: "0s" }} />
          <Cloud className="absolute top-40 right-[15%] w-16 h-16 text-accent/30 floating" style={{ animationDelay: "1s" }} />
          <Container className="absolute bottom-40 left-[20%] w-14 h-14 text-primary/30 floating" style={{ animationDelay: "2s" }} />
          <Terminal className="absolute top-60 left-[70%] w-12 h-12 text-accent/30 floating" style={{ animationDelay: "1.5s" }} />
          <Code2 className="absolute bottom-60 right-[25%] w-16 h-16 text-primary/30 floating" style={{ animationDelay: "0.5s" }} />
          <Cpu className="absolute top-80 left-[40%] w-12 h-12 text-accent/30 floating" style={{ animationDelay: "2.5s" }} />
        </div>

        <div className="relative z-10 text-center max-w-5xl mx-auto space-y-8 animate-fade-in-up">
          <div className="relative inline-block">
            <div className="w-48 h-48 mx-auto mb-8 rounded-full overflow-hidden border-4 border-primary/50 shadow-[0_0_50px_rgba(0,255,255,0.5)] animate-glow-pulse">
              <div className="w-full h-full bg-gradient-to-br from-primary/20 to-accent/20 flex items-center justify-center">
                <span className="text-4xl font-heading font-bold gradient-text">UK</span>
              </div>
            </div>
          </div>
          
          <h1 className="text-7xl md:text-8xl font-heading font-bold gradient-text mb-4">
            Uday Kiran Reddy
          </h1>
          
          <h2 className="text-3xl md:text-4xl font-heading text-foreground/90 mb-6">
            DevOps Engineer
          </h2>
          
          <p className="text-xl md:text-2xl text-muted-foreground font-light tracking-wide">
            Automation • Cloud • CI/CD • Linux • Docker
          </p>
          
          <Button 
            size="lg" 
            className="mt-8 bg-gradient-to-r from-primary to-accent text-primary-foreground hover:shadow-[0_0_30px_rgba(0,255,255,0.6)] transition-all duration-300 text-lg px-8 py-6 rounded-xl font-heading font-semibold"
          >
            <Download className="mr-2 w-5 h-5" />
            Download Resume
          </Button>
        </div>
      </section>

      {/* About Me Section */}
      <section className="py-20 px-4">
        <div className="max-w-4xl mx-auto">
          <h2 className="text-5xl font-heading font-bold text-center mb-16 gradient-text">About Me</h2>
          
          <Card className="glass-card p-8 md:p-12 space-y-6 hover:shadow-[0_0_50px_rgba(0,255,255,0.2)] transition-all duration-500">
            <div className="flex flex-col md:flex-row items-center gap-8">
              <div className="w-40 h-40 rounded-full overflow-hidden border-4 border-primary/40 shadow-[0_0_30px_rgba(0,255,255,0.4)] flex-shrink-0">
                <div className="w-full h-full bg-gradient-to-br from-primary/30 to-accent/30 flex items-center justify-center">
                  <span className="text-5xl font-heading font-bold gradient-text">UK</span>
                </div>
              </div>
              
              <div className="text-center md:text-left">
                <p className="text-lg leading-relaxed text-foreground/80">
                  I am <span className="text-primary font-semibold">Uday</span>, a DevOps Engineer specializing in 
                  <span className="text-accent font-semibold"> automation</span>, 
                  <span className="text-primary font-semibold"> cloud computing</span>, 
                  <span className="text-accent font-semibold"> containerization</span>, and building 
                  <span className="text-primary font-semibold"> scalable systems</span>. I enjoy working with 
                  Linux, AWS, CI/CD, Docker, Nginx, and creating efficient workflows for fast, reliable deployments.
                </p>
              </div>
            </div>
          </Card>
        </div>
      </section>

      {/* Skills Section */}
      <section className="py-20 px-4 bg-muted/20">
        <div className="max-w-6xl mx-auto">
          <h2 className="text-5xl font-heading font-bold text-center mb-16 gradient-text">Skills & Technologies</h2>
          
          <div className="flex flex-wrap justify-center gap-4">
            {skills.map((skill, index) => (
              <div
                key={skill}
                className="glass-card px-6 py-3 rounded-full border-2 border-primary/40 hover:border-primary hover:shadow-[0_0_20px_rgba(0,255,255,0.6)] transition-all duration-300 cursor-default animate-fade-in-up"
                style={{ animationDelay: `${index * 0.1}s` }}
              >
                <span className="text-lg font-heading font-semibold text-primary">
                  {skill}
                </span>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Projects Section */}
      <section className="py-20 px-4">
        <div className="max-w-6xl mx-auto">
          <h2 className="text-5xl font-heading font-bold text-center mb-16 gradient-text">
            <Cloud className="inline-block w-12 h-12 mb-2 mr-3 text-primary" />
            Projects
          </h2>
          
          <div className="grid md:grid-cols-2 gap-8">
            {/* Project 1: Nginx Reverse Proxy */}
            <Card className="glass-card p-8 hover:shadow-[0_0_50px_rgba(0,255,255,0.2)] transition-all duration-500 group">
              <div className="space-y-6">
                <h3 className="text-3xl font-heading font-bold text-primary group-hover:text-accent transition-colors">
                  Nginx Reverse Proxy Automation
                </h3>
                
                <p className="text-lg text-foreground/80 leading-relaxed">
                  Automated setup and deployment of Nginx as a reverse proxy for a Dockerized backend application. 
                  Included SSL configuration, load balancing, traffic routing, and container orchestration.
                </p>
                
                <div className="flex flex-wrap gap-3">
                  {["Nginx", "DevOps", "Docker", "Automation"].map((tag) => (
                    <span 
                      key={tag}
                      className="px-4 py-2 rounded-lg bg-primary/10 border border-primary/30 text-primary text-sm font-semibold"
                    >
                      {tag}
                    </span>
                  ))}
                </div>
                
                <Button 
                  className="mt-4 bg-gradient-to-r from-primary to-accent text-primary-foreground hover:shadow-[0_0_30px_rgba(0,255,255,0.6)] transition-all duration-300 font-heading font-semibold"
                >
                  View Project
                </Button>
              </div>
            </Card>

            {/* Project 2: Automated Backup System */}
            <Card className="glass-card p-8 hover:shadow-[0_0_50px_rgba(0,255,255,0.2)] transition-all duration-500 group">
              <div className="space-y-6">
                <h3 className="text-3xl font-heading font-bold text-primary group-hover:text-accent transition-colors">
                  Automated Backup System
                </h3>
                
                <p className="text-lg text-foreground/80 leading-relaxed">
                  Shell script-based backup automation with Cron scheduling. Takes daily/weekly backups of directories, 
                  compresses and uploads to AWS S3, and sends notifications upon completion.
                </p>
                
                <div className="flex flex-wrap gap-3">
                  {["Bash Scripting", "Cron", "Linux", "AWS S3"].map((tag) => (
                    <span 
                      key={tag}
                      className="px-4 py-2 rounded-lg bg-primary/10 border border-primary/30 text-primary text-sm font-semibold"
                    >
                      {tag}
                    </span>
                  ))}
                </div>
                
                <Button 
                  className="mt-4 bg-gradient-to-r from-primary to-accent text-primary-foreground hover:shadow-[0_0_30px_rgba(0,255,255,0.6)] transition-all duration-300 font-heading font-semibold"
                >
                  View Project
                </Button>
              </div>
            </Card>

            {/* Project 3: AWS Deployment Project */}
            <Card className="glass-card p-8 hover:shadow-[0_0_50px_rgba(0,255,255,0.2)] transition-all duration-500 group md:col-span-2">
              <div className="space-y-6">
                <h3 className="text-3xl font-heading font-bold text-primary group-hover:text-accent transition-colors">
                  <Cloud className="inline-block w-8 h-8 mr-2 mb-1" />
                  AWS Deployment Project
                </h3>
                
                <p className="text-lg text-foreground/80 leading-relaxed">
                  Full-stack AWS cloud deployment project implementing EC2 instances, S3 storage, IAM roles, and VPC configuration 
                  for secure and scalable application hosting.
                </p>
                
                <div className="grid md:grid-cols-2 gap-4 my-6">
                  <div className="flex items-start gap-3">
                    <Server className="w-5 h-5 text-accent mt-1 flex-shrink-0" />
                    <div>
                      <h4 className="font-semibold text-accent mb-1">EC2 Deployment</h4>
                      <p className="text-sm text-foreground/70">Deploy applications on EC2 instances</p>
                    </div>
                  </div>
                  <div className="flex items-start gap-3">
                    <Cloud className="w-5 h-5 text-accent mt-1 flex-shrink-0" />
                    <div>
                      <h4 className="font-semibold text-accent mb-1">S3 Storage</h4>
                      <p className="text-sm text-foreground/70">Static content storage and CDN</p>
                    </div>
                  </div>
                  <div className="flex items-start gap-3">
                    <Container className="w-5 h-5 text-accent mt-1 flex-shrink-0" />
                    <div>
                      <h4 className="font-semibold text-accent mb-1">IAM Security</h4>
                      <p className="text-sm text-foreground/70">Secure IAM roles and policies</p>
                    </div>
                  </div>
                  <div className="flex items-start gap-3">
                    <Terminal className="w-5 h-5 text-accent mt-1 flex-shrink-0" />
                    <div>
                      <h4 className="font-semibold text-accent mb-1">VPC Configuration</h4>
                      <p className="text-sm text-foreground/70">Network setup with security groups</p>
                    </div>
                  </div>
                </div>
                
                <div className="flex flex-wrap gap-3">
                  {["AWS Cloud", "EC2", "S3", "IAM", "VPC", "Security Groups"].map((tag) => (
                    <span 
                      key={tag}
                      className="px-4 py-2 rounded-lg bg-primary/10 border border-primary/30 text-primary text-sm font-semibold"
                    >
                      {tag}
                    </span>
                  ))}
                </div>
                
                <Button 
                  className="mt-4 bg-gradient-to-r from-primary to-accent text-primary-foreground hover:shadow-[0_0_30px_rgba(0,255,255,0.6)] transition-all duration-300 font-heading font-semibold"
                >
                  View Project
                </Button>
              </div>
            </Card>
          </div>
        </div>
      </section>

      {/* Timeline Section */}
      <section className="py-20 px-4 bg-muted/20">
        <div className="max-w-3xl mx-auto">
          <h2 className="text-5xl font-heading font-bold text-center mb-16 gradient-text">
            <Cloud className="inline-block w-12 h-12 mb-2 mr-3 text-accent" />
            My Journey
          </h2>
          
          <div className="relative">
            {/* Vertical Line */}
            <div className="absolute left-8 top-0 bottom-0 w-0.5 bg-gradient-to-b from-primary via-accent to-primary" />
            
            <div className="space-y-12">
              {timeline.map((item, index) => (
                <div 
                  key={index}
                  className="relative pl-20 animate-fade-in-up"
                  style={{ animationDelay: `${index * 0.15}s` }}
                >
                  {/* Timeline Dot */}
                  <div className="absolute left-6 w-5 h-5 rounded-full bg-primary shadow-[0_0_20px_rgba(0,255,255,0.8)] border-4 border-background" />
                  
                  <Card className="glass-card p-6 hover:shadow-[0_0_30px_rgba(0,255,255,0.2)] transition-all duration-300">
                    <div className="flex flex-col sm:flex-row sm:items-center gap-4">
                      <span className="text-2xl font-heading font-bold text-accent min-w-[80px]">
                        {item.year}
                      </span>
                      <span className="text-lg text-foreground/80">
                        {item.event}
                      </span>
                    </div>
                  </Card>
                </div>
              ))}
            </div>
          </div>
        </div>
      </section>

      {/* Contact Section */}
      <section className="py-20 px-4">
        <div className="max-w-3xl mx-auto">
          <h2 className="text-5xl font-heading font-bold text-center mb-16 gradient-text">Get In Touch</h2>
          
          <Card className="glass-card p-8 md:p-12 hover:shadow-[0_0_50px_rgba(0,255,255,0.2)] transition-all duration-500">
            <div className="space-y-8">
              <div className="flex items-center gap-6 group cursor-pointer">
                <div className="w-16 h-16 rounded-full bg-primary/20 flex items-center justify-center group-hover:shadow-[0_0_20px_rgba(0,255,255,0.6)] transition-all duration-300">
                  <Mail className="w-8 h-8 text-primary" />
                </div>
                <div>
                  <p className="text-sm text-muted-foreground mb-1">Email</p>
                  <a 
                    href="mailto:gudaykiran3890@gmail.com"
                    className="text-xl font-heading font-semibold text-primary hover:text-accent transition-colors"
                  >
                    gudaykiran3890@gmail.com
                  </a>
                </div>
              </div>
              
              <div className="flex items-center gap-6 group cursor-pointer">
                <div className="w-16 h-16 rounded-full bg-accent/20 flex items-center justify-center group-hover:shadow-[0_0_20px_rgba(168,85,247,0.6)] transition-all duration-300">
                  <Linkedin className="w-8 h-8 text-accent" />
                </div>
                <div>
                  <p className="text-sm text-muted-foreground mb-1">LinkedIn</p>
                  <a 
                    href="https://www.linkedin.com/in/gorla-uday-kiran-reddy-364006259/"
                    target="_blank"
                    rel="noopener noreferrer"
                    className="text-xl font-heading font-semibold text-accent hover:text-primary transition-colors"
                  >
                    Connect with me
                  </a>
                </div>
              </div>
            </div>
          </Card>
        </div>
      </section>

      {/* Footer */}
      <footer className="relative py-8 px-4 border-t-2 border-primary/30">
        <div className="absolute inset-x-0 top-0 h-0.5 bg-gradient-to-r from-transparent via-primary to-transparent" />
        
        <p className="text-center text-muted-foreground">
          © 2025 <span className="text-primary font-semibold">Uday Kiran Reddy</span> — DevOps Engineer | All Rights Reserved
        </p>
      </footer>
    </div>
  );
};

export default Index;
