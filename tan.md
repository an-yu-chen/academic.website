body {
    font-family: 'Georgia', serif;
    line-height: 1.6;
    margin: 0;
    padding: 0;
    background-color: #f4f0e8; /* A warm, creamy background */
    color: #333;
}

.journey-header {
    background-color: #e0ac8f; /* A soft, earthy terracotta colour */
    color: #fff;
    text-align: center;
    padding: 2.5rem 0;
    margin-bottom: 2rem;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}

.journey-header h1 {
    margin: 0;
    font-size: 2.5rem;
    letter-spacing: 0.1rem;
}

.journey-content {
    max-width: 900px;
    margin: 0 auto;
    padding: 0 1.5rem;
}

section {
    margin-bottom: 2.5rem;
}

.journey-image {
    display: block;
    max-width: 100%;
    height: auto;
    border-radius: 10px; /* A subtle curve on the corners */
    margin: 1.5rem auto;
    box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    border: 3px solid #e0ac8f; /* A complementary border colour */
}

p {
    text-align: justify;
    margin-bottom: 1rem;
}

hr {
    border: none;
    height: 1px;
    background-color: #e0ac8f;
    margin: 3rem 0;
}

.journey-footer {
    text-align: center;
    padding: 1.5rem;
    background-color: #5d493a; /* A darker brown for contrast */
    color: #fff;
    margin-top: 3rem;
}

.journey-footer p {
    margin: 0;
    font-size: 0.9rem;
}

@media (min-width: 768px) {
    .intro-section, .learning-section {
        display: flex;
        align-items: center;
        gap: 2rem;
    }

    .intro-section .journey-image {
        order: 1;
        width: 50%;
    }

    .learning-section .journey-image {
        order: 2;
        width: 50%;
    }
}
