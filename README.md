import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Badge } from "@/components/ui/badge";
import { Button } from "@/components/ui/button";
import { Mail, Phone, Linkedin, Github, Globe } from "lucide-react";

export default function Portfolio() {
  return (
    <div className="grid grid-cols-12 min-h-screen">
      {/* Left Panel */}
      <aside className="col-span-3 bg-gray-100 p-6 border-r border-gray-300">
        <h1 className="text-2xl font-bold mb-2">Sarthak Verma</h1>
        <p className="text-sm text-gray-600 mb-4">Dallas, TX | AI | Analytics | Product</p>
        <ul className="space-y-2">
          <li className="flex items-center gap-2 text-sm"><Linkedin size={16} /> <a href="https://www.linkedin.com/in/sarthakmverma" target="_blank">LinkedIn</a></li>
          <li className="flex items-center gap-2 text-sm"><Github size={16} /> <a href="https://github.com/sarthakmverma" target="_blank">GitHub</a></li>
          <li className="flex items-center gap-2 text-sm"><Globe size={16} /> <a href="https://sarthakmverma.github.io/portfolio" target="_blank">Portfolio</a></li>
          <li className="flex items-center gap-2 text-sm"><Mail size={16} /> sarthak.verma@utdallas.edu</li>
          <li className="flex items-center gap-2 text-sm"><Phone size={16} /> 945-274-8299</li>
        </ul>
      </aside>

      {/* Main Content */}
      <main className="col-span-9 p-8 space-y-8 overflow-y-auto">
        <section>
          <h2 className="text-xl font-semibold mb-2">About Me</h2>
          <p className="text-gray-700">Product-minded program manager focused on AI-driven innovation, analytics execution, and seamless digital experiences. Experienced in transforming business needs into scalable solutions through a blend of technical depth and strategic product thinking. Built payment platforms, onboarding flows, and BI systems across Sabre, Capital One, and startups. I thrive at the intersection of data, design, and delivery.</p>
        </section>

        <section>
          <h2 className="text-xl font-semibold mb-2">Skills</h2>
          <div className="space-y-2">
            <div>
              <h3 className="font-medium">Data & Analytics</h3>
              <div className="flex flex-wrap gap-2">
                <Badge>Python</Badge><Badge>R</Badge><Badge>SQL</Badge><Badge>TensorFlow</Badge><Badge>SAS</Badge><Badge>Power BI</Badge><Badge>Tableau</Badge>
              </div>
            </div>
            <div>
              <h3 className="font-medium">Cloud & Infra</h3>
              <div className="flex flex-wrap gap-2">
                <Badge>AWS</Badge><Badge>GCP</Badge><Badge>Snowflake</Badge><Badge>MongoDB</Badge>
              </div>
            </div>
            <div>
              <h3 className="font-medium">Product Tools</h3>
              <div className="flex flex-wrap gap-2">
                <Badge>Jira</Badge><Badge>Confluence</Badge><Badge>Figma</Badge><Badge>Alteryx</Badge><Badge>Excel</Badge>
              </div>
            </div>
          </div>
        </section>

        <section>
          <h2 className="text-xl font-semibold mb-2">Experience</h2>
          <Card>
            <CardContent className="pt-4">
              <h3 className="font-bold">Sabre Corporation – Program Analytics Intern</h3>
              <p className="text-sm text-gray-600">May–Aug 2024</p>
              <ul className="list-disc list-inside mt-2 text-gray-700">
                <li>Boosted booking efficiency by 15% using SQL on GDS data</li>
                <li>Developed Power BI dashboards, cutting reporting lag by 30%</li>
                <li>Built forecasting models, improving prediction accuracy by 20%</li>
              </ul>
            </CardContent>
          </Card>
          <Card>
            <CardContent className="pt-4">
              <h3 className="font-bold">Capgemini @ Capital One – Program Manager</h3>
              <p className="text-sm text-gray-600">Jun 2021 – Jun 2023</p>
              <ul className="list-disc list-inside mt-2 text-gray-700">
                <li>Reduced onboarding time by 20% using automation</li>
                <li>Analyzed 150K+ records with TensorFlow/SAS to detect fraud</li>
                <li>Closed $6M+ revenue via stakeholder demos and GTM</li>
              </ul>
            </CardContent>
          </Card>
          <Card>
            <CardContent className="pt-4">
              <h3 className="font-bold">The Mohh – Program Manager</h3>
              <p className="text-sm text-gray-600">Jun 2018 – Jun 2021</p>
              <ul className="list-disc list-inside mt-2 text-gray-700">
                <li>Led sprints to develop real-time payment dashboards</li>
                <li>Built compliant features for secure payment visibility</li>
                <li>Collaborated with engineers to improve client UX</li>
              </ul>
            </CardContent>
          </Card>
        </section>

        <section>
          <h2 className="text-xl font-semibold mb-2">Projects</h2>
          <ul className="list-disc list-inside text-gray-700">
            <li><strong>BullsI:</strong> Built real-time AI alert system for schools, saving $10K/incident</li>
            <li><strong>Digital Onboarding:</strong> Created platform scaling to 5K+ users with 10% MoM growth</li>
          </ul>
        </section>

        <section>
          <h2 className="text-xl font-semibold mb-2">Education</h2>
          <p className="text-gray-700">M.S. Business Analytics & AI, UTD (2023–2025)<br/>B.E. ECE, SVVV Indore (2016–2020)</p>
        </section>

        <section>
          <h2 className="text-xl font-semibold mb-2">Awards & Certifications</h2>
          <ul className="list-disc list-inside text-gray-700">
            <li>Hosted UTD career fair with 12+ companies</li>
            <li>"Most Innovative Product" – Capgemini POC</li>
            <li>CSPO®, GenAI for PMs, Pendo Product Analytics, Alteryx, Deep Learning</li>
          </ul>
        </section>

        <footer className="pt-8">
          <Button variant="outline" asChild>
            <a href="https://sarthakmverma.github.io/portfolio/Sarthak_Verma_Resume.pdf" target="_blank">Download Resume</a>
          </Button>
        </footer>
      </main>
    </div>
  );
}
