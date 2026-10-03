* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: #f4f6fb;
    color: #1f2937;
    line-height: 1.6;
}

.container {
    width: min(1100px, 90%);
    margin: 0 auto;
}

.navbar {
    background: linear-gradient(135deg, #4f46e5, #7c3aed);
    position: sticky;
    top: 0;
    z-index: 10;
    box-shadow: 0 2px 8px rgba(0,0,0,0.08);
}

.navbar .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 0;
}

.logo {
    color: white;
    font-size: 1.5rem;
}

.nav-links {
    list-style: none;
    display: flex;
    gap: 1.5rem;
    flex-wrap: wrap;
}

.nav-links a {
    color: white;
    text-decoration: none;
    font-weight: 500;
}

.hero {
    background: linear-gradient(135deg, #4f46e5, #7c3aed);
    color: white;
    text-align: center;
    padding: 7rem 0;
}

.hero h2 {
    font-size: clamp(2.2rem, 4vw, 4rem);
    margin-bottom: 0.8rem;
}

.hero p {
    font-size: 1.2rem;
    margin-bottom: 1.5rem;
}

.btn {
    display: inline-block;
    background: white;
    color: #4f46e5;
    text-decoration: none;
    padding: 0.9rem 1.7rem;
    border-radius: 999px;
    font-weight: bold;
    transition: 0.2s ease;
}

.btn:hover {
    transform: translateY(-2px);
}

.about,
.projects,
.skills,
.contact {
    padding: 5rem 0;
}

.about h2,
.projects h2,
.skills h2,
.contact h2 {
    text-align: center;
    font-size: 2rem;
    margin-bottom: 1.5rem;
    color: #1f2937;
}

.about p {
    max-width: 800px;
    margin: 0 auto 1rem;
    text-align: center;
    font-size: 1.05rem;
    color: #374151;
}

.section-subtitle {
    text-align: center;
    margin-bottom: 2rem;
    color: #4b5563;
}

.projects-grid,
.skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
}

.project-card,
.skill-item {
    background: white;
    border-radius: 12px;
    padding: 1.5rem;
    box-shadow: 0 6px 18px rgba(0,0,0,0.05);
}

.project-card h3,
.skill-item h4 {
    color: #4f46e5;
    margin-bottom: 0.8rem;
}

.project-card p,
.skill-item p {
    color: #4b5563;
}

.tech {
    margin-top: 0.8rem;
    font-style: italic;
    color: #6b7280;
}

.project-link {
    display: inline-block;
    margin-top: 1rem;
    color: #4f46e5;
    text-decoration: none;
    font-weight: 600;
}

.contact {
    background: #eef2ff;
    text-align: center;
}

.contact p {
    max-width: 650px;
    margin: 0 auto 2rem;
    color: #374151;
}

.contact-info {
    display: flex;
    justify-content: center;
    gap: 1rem;
    flex-wrap: wrap;
}

.contact-link {
    background: #4f46e5;
    color: white;
    text-decoration: none;
    padding: 0.8rem 1.3rem;
    border-radius: 999px;
    font-weight: 600;
}

footer {
    background: #111827;
    color: white;
    text-align: center;
    padding: 1.5rem 0;
}

@media (max-width: 700px) {
    .navbar .container {
        flex-direction: column;
        gap: 0.8rem;
    }

    .nav-links {
        justify-content: center;
    }

    .hero {
        padding: 5rem 0;
    }
}
