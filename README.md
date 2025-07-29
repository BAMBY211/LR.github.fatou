<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>BambyLove - Produits Naturels à l'Aloe Vera</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
	<head>
    <link rel="stylesheet" href="style.css">
</head>
    <style>
        :root {
            --primary: #2a2a2a;
            --secondary: #d4af37;
            --light: #f8f9fa;
            --dark: #212529;
            --text: #333;
            --transition: all 0.3s ease;
        }
        
    /* ===== CORRECTION CSS RESPONSIVE COMPLÈTE ===== */

/* 1. Réinitialisation de base */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* 2. Styles généraux responsives */
body {
    font-family: 'Montserrat', sans-serif;
    line-height: 1.6;
    font-size: 16px;
    overflow-x: hidden;
    color: #333;
}

/* 3. Conteneur principal responsive */
.container {
    width: 100%;
    max-width: 1400px;
    margin: 0 auto;
    padding: 0 15px;
}

/* 4. Correction spécifique pour hero-slide */
.hero-slide {
    position: relative;
    width: 100%;
    height: 0;
    padding-bottom: 40%; /* Ratio 5:2 pour le slider */
    overflow: hidden;
}

.hero-slide img {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: center;
}

/* 5. Système de grille responsive */
.products-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1rem;
    padding: 1rem;
}

/* 6. Cartes de produits responsive */
.product-card {
    background: white;
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 3px 10px rgba(0,0,0,0.1);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.product-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 5px 15px rgba(0,0,0,0.2);
}

/* 7. Media Queries pour différents écrans */

/* Mobile (par défaut) */
@media (max-width: 767px) {
    body {
        font-size: 14px;
    }
    
    .hero-slide {
        padding-bottom: 60%; /* Ratio plus carré pour mobile */
    }
}

/* Tablettes */
@media (min-width: 768px) and (max-width: 1023px) {
    .products-grid {
        grid-template-columns: repeat(2, 1fr);
    }
    
    .hero-slide {
        padding-bottom: 50%;
    }
}

/* Petits écrans d'ordinateur */
@media (min-width: 1024px) and (max-width: 1279px) {
    .products-grid {
        grid-template-columns: repeat(3, 1fr);
    }
}

/* Grands écrans */
@media (min-width: 1280px) {
    .products-grid {
        grid-template-columns: repeat(4, 1fr);
    }
}

/* 8. Corrections spécifiques pour iOS */
@supports (-webkit-touch-callout: none) {
    .hero-slide {
        height: 50vh; /* Solution de repli pour Safari */
    }
}

/* 9. Optimisation des images */
img {
    max-width: 100%;
    height: auto;
    vertical-align: middle;
}

/* 10. Typographie responsive */
h1 {
    font-size: 2rem;
    line-height: 1.2;
    margin-bottom: 1rem;
}

h2 {
    font-size: 1.75rem;
}

@media (min-width: 768px) {
    h1 {
        font-size: 2.5rem;
    }
    
    h2 {
        font-size: 2rem;
    }
}

/* 11. Espacement responsive */
.section {
    padding: 2rem 1rem;
}

@media (min-width: 768px) {
    .section {
        padding: 3rem 2rem;
    }
}

/* 12. Navigation responsive */
.navbar {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
    padding: 1rem;
}

/* 13. Boutons responsive */
.btn {
    display: inline-block;
    padding: 0.75rem 1.5rem;
    font-size: 1rem;
    border-radius: 50px;
    transition: all 0.3s ease;
}

@media (max-width: 767px) {
    .btn {
        width: 100%;
        text-align: center;
    }
}
        }

        .payment-text {
            opacity: 0.7;
        }
        .payment-text {
            background: linear-gradient(90deg, 
                        rgba(255,255,255,0.5), 
                        rgba(255,255,255,0.8));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
    </style>
</head>
<body>
<script>
// Script pour le diaporama
document.addEventListener("DOMContentLoaded", function () {
    const slides = document.querySelectorAll(".hero-slide");
    let currentSlide = 0;

    function showSlide(index) {
        slides.forEach((slide, i) => {
            slide.classList.toggle("active", i === index);
        });
    }

    function nextSlide() {
        currentSlide = (currentSlide + 1) % slides.length;
        showSlide(currentSlide);
    }

    // Afficher la première image
    showSlide(currentSlide);

    // Changer d'image toutes les 5 secondes
    setInterval(nextSlide, 5000);
});
</script>
    <!-- Navigation -->
    <nav class="navbar">
        <div class="logo-container">
            <a href="#" class="logo">FATOU<span>LOVE</span></a>
            <img src="66.jpg" alt="Logo BambyLove" class="nav-logo">
        </div>
        <div class="nav-links">
            <a href="LR.html">Accueil</a>
            <a href="Sert.html">Produits</a>
            <a href="Ppo.html">À propos</a>
            <a href="Ret.html">Contact</a>
        </div>
    </nav>
<!-- Hero Section -->
<section class="hero">
    <div class="hero-slideshow">
	    <div class="hero-slide"><img src="233.jpg" alt="Slide 3"></div>
        <!-- Ajoutez autant d'images que nécessaire -->
    </div>
    <div class="hero-content">
        <h1>Collection Exclusive 2025</h1>
        <p>Découvrez notre sélection de produits naturels à l'Aloe Vera, alliant bien-être et qualité exceptionnelle.</p>
        <a href="#products" class="btn">Explorer la collection</a>
    </div>
</section>
  

    <!-- Products Section -->
    <section class="products-section" id="products">
        <div class="section-title">
            <h2>Nos Produits Phares</h2>
        </div>
        <div class="products-grid">
            <!-- Produit 1 -->
            <div class="product-card">
                <div class="product-badge">Nouveau</div>
                <div class="product-img-container">
                    <img src="50.jpg" alt="Health and Beauty Gel" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Health and Beauty Gel pour Homme</h3>
                    <p class="product-price">19,90 €</p>
                    <p class="product-price-fcfa">≈ 13 035 FCFA</p>
                    <p class="product-description">Gel hydratant à base d'aloe vera pour une peau saine et rafraîchie.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>

            <!-- Produit 2 -->
            <div class="product-card">
                <div class="product-badge">Best-seller</div>
                <div class="product-img-container">
                    <img src="52.jpg" alt="Aloe Vera Drinking Gel" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Aloe Vera Drinking Gel</h3>
                    <p class="product-price">22,50 €</p>
                    <p class="product-price-fcfa">≈ 14 738 FCFA</p>
                    <p class="product-description">Gel à boire à l'aloe vera avec gingembre, citron et miel.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>

            <!-- Produit 3 -->
            <div class="product-card">
                <div class="product-badge">Best-seller</div>
                <div class="product-img-container">
                    <img src="53.jpeg" alt="Lotion et Shampoing pour Bébé" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Lotion et Shampoing pour Bébé</h3>
                    <p class="product-price">16,90 €</p>
                    <p class="product-price-fcfa">≈ 11 070 FCFA</p>
                    <p class="product-description">Produits doux sans parfum pour la peau délicate des bébés.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>
            
            <!-- Produit 4 -->
            <div class="product-card">
                <div class="product-badge">Best-seller</div>
                <div class="product-img-container">
                    <img src="67.jpg" alt="Crème correctrice" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Crème correctrice Aloe Vera</h3>
                    <p class="product-price">24,90 €</p>
                    <p class="product-price-fcfa">≈ 16 310 FCFA</p>
                    <p class="product-description">Crème réparatrice pour les imperfections cutanées.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>
            
            <!-- Produit 5 -->
            <div class="product-card">
                <div class="product-badge">Nouveauté</div>
                <div class="product-img-container">
                    <img src="60.jpg" alt="Gel Visage Possiflore bleue" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Gel Visage Possiflore</h3>
                    <p class="product-price">18,50 €</p>
                    <p class="product-price-fcfa">≈ 12 118 FCFA</p>
                    <p class="product-description">Gel rafraîchissant pour le visage à la fleur de passiflore.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>
            
            <!-- Produit 6 -->
            <div class="product-card">
                <div class="product-badge">Promo</div>
                <div class="product-img-container">
                    <img src="59.jpg" alt="Exotic Papaya" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Exotic Papaya</h3>
                    <p class="product-price"><del>25,00 €</del> 19,90 €</p>
                    <p class="product-price-fcfa"><del>≈ 16 375 FCFA</del> ≈ 13 035 FCFA</p>
                    <p class="product-description">Soin exfoliant à la papaye pour une peau lumineuse.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>
            
            <!-- Produit 7 -->
            <div class="product-card">
                <div class="product-badge">Best-seller</div>
                <div class="product-img-container">
                    <img src="54.jpg" alt="Lait nettoyant Visage" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Lait nettoyant Visage</h3>
                    <p class="product-price">15,90 €</p>
                    <p class="product-price-fcfa">≈ 10 415 FCFA</p>
                    <p class="product-description">Nettoyant doux pour le visage à l'Aloe Vera.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>
            
            <!-- Produit 8 -->
            <div class="product-card">
                <div class="product-badge">Édition limitée</div>
                <div class="product-img-container">
                    <img src="55.jpg" alt="Sérum Aloe Vera" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Sérum Aloe Vera</h3>
                    <p class="product-price">29,90 €</p>
                    <p class="product-price-fcfa">≈ 19 585 FCFA</p>
                    <p class="product-description">Sérum intensif pour une hydratation profonde.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>
            
            <!-- Produit 9 -->
            <div class="product-card">
                <div class="product-badge">Nouveau</div>
                <div class="product-img-container">
                    <img src="76.jpg" alt="24h Moisture Face Serum" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">24h Moisture Face Serum</h3>
                    <p class="product-price">27,50 €</p>
                    <p class="product-price-fcfa">≈ 18 013 FCFA</p>
                    <p class="product-description">Sérum hydratant longue durée à l'Aloe Vera.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>
            
            <!-- Produit 10 -->
            <div class="product-card">
                <div class="product-badge">Nouveauté</div>
                <div class="product-img-container">
                    <img src="51.jpg" alt="Crème hydratante" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Crème Hydratante Aloe</h3>
                    <p class="product-price">17,90 €</p>
                    <p class="product-price-fcfa">≈ 11 725 FCFA</p>
                    <p class="product-description">Crème nourrissante à base d'aloe vera pour une peau douce.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>
            
            <!-- Produit 11 -->
            <div class="product-card">
                <div class="product-badge">Édition limitée</div>
                <div class="product-img-container">
                    <img src="57.jpg" alt="Kit Soin Complet" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Kit Soin Complet</h3>
                    <p class="product-price">49,90 €</p>
                    <p class="product-price-fcfa">≈ 32 685 FCFA</p>
                    <p class="product-description">Kit complet pour une routine de soin à l'Aloe Vera.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>
            <!-- Produit 12 -->
            <div class="product-card">
                <div class="product-badge">Nouveau</div>
                <div class="product-img-container">
                    <img src="01.jpeg" alt="Shampoing Aloe Vera" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Shampoing Purifiant Aloe Vera</h3>
                    <p class="product-price">18,90 €</p>
                    <p class="product-price-fcfa">≈ 12 380 FCFA</p>
                    <p class="product-description">Shampoing doux à l'Aloe Vera pour cuir chevelu sain et cheveux brillants.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>

            <!-- Produit 13 -->
            <div class="product-card">
                <div class="product-badge">Best-seller</div>
                <div class="product-img-container">
                    <img src="05.jpeg" alt="Masque Visage Aloe Vera" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Masque Apaisant Aloe Vera</h3>
                    <p class="product-price">21,50 €</p>
                    <p class="product-price-fcfa">≈ 14 083 FCFA</p>
                    <p class="product-description">Masque hydratant et apaisant pour peau sensible et irritée.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>

            <!-- Produit 14 -->
            <div class="product-card">
                <div class="product-badge">Édition limitée</div>
                <div class="product-img-container">
                    <img src="03.jpg" alt="Lotion Après-Soleil" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Lotion Après-Soleil Aloe Vera</h3>
                    <p class="product-price">23,90 €</p>
                    <p class="product-price-fcfa">≈ 15 655 FCFA</p>
                    <p class="product-description">Apaisement immédiat pour les peaux exposées au soleil.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>

            <!-- Produit 15 -->
            <div class="product-card">
                <div class="product-badge">Nouveauté</div>
                <div class="product-img-container">
                    <img src="04.jpg" alt="Déodorant Naturel" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Déodorant Naturel Aloe Vera</h3>
                    <p class="product-price">14,90 €</p>
                    <p class="product-price-fcfa">≈ 9 760 FCFA</p>
                    <p class="product-description">Déodorant sans aluminium à l'Aloe Vera et huile de coco.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>

            <!-- Produit 16 -->
            <div class="product-card">
                <div class="product-badge">Promo</div>
                <div class="product-img-container">
                    <img src="06.jpg" alt="Tonique Visage" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Tonique Raffermissant Aloe Vera</h3>
                    <p class="product-price"><del>19,90 €</del> 16,50 €</p>
                    <p class="product-price-fcfa"><del>≈ 13 035 FCFA</del> ≈ 10 808 FCFA</p>
                    <p class="product-description">Tonique purifiant pour pores resserrés et peau tonifiée.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>

            <!-- Produit 17 -->
            <div class="product-card">
                <div class="product-badge">Best-seller</div>
                <div class="product-img-container">
                    <img src="07.png" alt="Soin Pieds" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Crème Pieds Secs Aloe Vera</h3>
                    <p class="product-price">15,90 €</p>
                    <p class="product-price-fcfa">≈ 10 415 FCFA</p>
                    <p class="product-description">Crème réparatrice intensive pour pieds très secs.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>

            <!-- Produit 18 -->
            <div class="product-card">
                <div class="product-badge">Nouveau</div>
                <div class="product-img-container">
                    <img src="009.png" alt="Démaquillant" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Lait Démaquillant Aloe Vera</h3>
                    <p class="product-price">17,50 €</p>
                    <p class="product-price-fcfa">≈ 11 463 FCFA</p>
                    <p class="product-description">Démaquille en douceur tout en hydratant la peau.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>

            <!-- Produit 19 -->
            <div class="product-card">
                <div class="product-badge">Édition limitée</div>
                <div class="product-img-container">
                    <img src="008.png" alt="Lotion Corporelle" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Lotion Corporelle Aloe Vera</h3>
                    <p class="product-price">22,90 €</p>
                    <p class="product-price-fcfa">≈ 15 000 FCFA</p>
                    <p class="product-description">Hydratation intense pour le corps, absorption rapide.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>

            <!-- Produit 20 -->
            <div class="product-card">
                <div class="product-badge">Pack</div>
                <div class="product-img-container">
                    <img src="007.jpg" alt="Pack Découverte" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Pack Découverte Aloe Vera</h3>
                    <p class="product-price">39,90 €</p>
                    <p class="product-price-fcfa">≈ 26 135 FCFA</p>
                    <p class="product-description">Sélection de nos meilleurs produits pour une routine complète.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>
            <!-- Produit 21 -->
            <div class="product-card">
                <div class="product-badge">Nouveauté</div>
                <div class="product-img-container">
                    <img src="223.png" alt="Gel Intime Aloe Vera" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Emergency Spray Flacon Vide 30ml</h3>
                    <p class="product-price">16,90 €</p>
                    <p class="product-price-fcfa">≈ 11 070 FCFA</p>
                    <p class="product-description">Gel nettoyant doux pH neutre pour une hygiène intime respectueuse.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>

            <!-- Produit 22 -->
            <div class="product-card">
                <div class="product-badge">Best-seller</div>
                <div class="product-img-container">
                    <img src="224.png" alt="Dentifrice Aloe Vera" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Aloe Vera Gel à Boire Active Freedom LR – Soutien Articulaire</h3>
                    <p class="product-price">9,90 €</p>
                    <p class="product-price-fcfa">≈ 6 485 FCFA</p>
                    <p class="product-description">Dentifrice naturel au pouvoir blanchissant et apaisant pour les gencives.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>

            <!-- Produit 23 -->
            <div class="product-card">
                <div class="product-badge">Édition limitée</div>
                <div class="product-img-container">
                    <img src="225.jpg" alt="Huile Massage Aloe Vera" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Huile Massage Aloe Vera</h3>
                    <p class="product-price">26,50 €</p>
                    <p class="product-price-fcfa">≈ 17 358 FCFA</p>
                    <p class="product-description">Huile de massage relaxante enrichie en Aloe Vera et huiles essentielles.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>

            <!-- Produit 24 -->
            <div class="product-card">
                <div class="product-badge">Nouveau</div>
                <div class="product-img-container">
                    <img src="226.png" alt="Gommage Corps Aloe Vera" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Gommage Corps Aloe Vera</h3>
                    <p class="product-price">18,90 €</p>
                    <p class="product-price-fcfa">≈ 12 380 FCFA</p>
                    <p class="product-description">Gommage exfoliant doux pour une peau lisse et radieuse.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>

            <!-- Produit 25 -->
            <div class="product-card">
                <div class="product-badge">Promo</div>
                <div class="product-img-container">
                    <img src="227.jpg" alt="Spray Hydratant Aloe Vera" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Spray Hydratant Aloe Vera</h3>
                    <p class="product-price"><del>14,90 €</del> 12,50 €</p>
                    <p class="product-price-fcfa"><del>≈ 9 760 FCFA</del> ≈ 8 188 FCFA</p>
                    <p class="product-description">Brume fraîcheur pour un coup d'éclat instantané toute la journée.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>

            <!-- Produit 26 -->
            <div class="product-card">
                <div class="product-badge">Best-seller</div>
                <div class="product-img-container">
                    <img src="228.jpg" alt="Baume à Lèvres Aloe Vera" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Baume à Lèvres Aloe Vera</h3>
                    <p class="product-price">6,90 €</p>
                    <p class="product-price-fcfa">≈ 4 520 FCFA</p>
                    <p class="product-description">Soin réparateur intensif pour lèvres gercées et sèches.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>

            <!-- Produit 27 -->
            <div class="product-card">
                <div class="product-badge">Nouveauté</div>
                <div class="product-img-container">
                    <img src="229.png" alt="Gel Jambes Lourdes Aloe Vera" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Gel Jambes Lourdes Aloe Vera</h3>
                    <p class="product-price">21,90 €</p>
                    <p class="product-price-fcfa">≈ 14 345 FCFA</p>
                    <p class="product-description">Sensation de fraîcheur immédiate pour jambes fatiguées.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>

            <!-- Produit 28 -->
            <div class="product-card">
                <div class="product-badge">Éco-responsable</div>
                <div class="product-img-container">
                    <img src="230.png" alt="Savon Liquide Aloe Vera" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Savon Liquide Aloe Vera</h3>
                    <p class="product-price">12,90 €</p>
                    <p class="product-price-fcfa">≈ 8 450 FCFA</p>
                    <p class="product-description">Nettoyant corporel doux sans savon, pH neutre.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>

            <!-- Produit 29 -->
            <div class="product-card">
                <div class="product-badge">Détente</div>
                <div class="product-img-container">
                    <img src="231.png" alt="Compresses Oculaires Aloe Vera" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Compresses Oculaires Aloe Vera</h3>
                    <p class="product-price">15,50 €</p>
                    <p class="product-price-fcfa">≈ 10 153 FCFA</p>
                    <p class="product-description">Apaisement immédiat pour les yeux fatigués.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>

            <!-- Produit 30 -->
            <div class="product-card">
                <div class="product-badge">Pour Homme</div>
                <div class="product-img-container">
                    <img src="232.jpg" alt="Stick à Raser Aloe Vera" class="product-img">
                </div>
                <div class="product-info">
                    <h3 class="product-title">Stick à Raser Aloe Vera</h3>
                    <p class="product-price">13,90 €</p>
                    <p class="product-price-fcfa">≈ 9 105 FCFA</p>
                    <p class="product-description">Prévient les irritations et les rougeons après rasage.</p>
                    <div class="product-actions">
                        <button class="wishlist-btn"><i class="far fa-heart"></i></button>
                        <a href="#" class="btn">Voir détails</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="footer-content">
            <div class="footer-column">
                <h3>BAMBYLOVE</h3>
                <p>Nous offrons des produits naturels de haute qualité pour votre bien-être.</p>
                <div class="social-links">
                    <a href="https://facebook.com/ascesw.pasvraiment" target="_blank" title="Facebook"><i class="fab fa-facebook-f"></i></a>
                    <a href="https://www.instagram.com/bamby_diop21/"><i class="fab fa-instagram"></i></a>
                    <a href="https://www.tiktok.com/@abd221.com"><i class="fab fa-tiktok"></i></a>
                    <a href="https://wa.me/773767317" target="_blank"><i class="fab fa-whatsapp"></i></a>
                </div>
            </div>
            <div class="footer-column">
                <h3>Liens utiles</h3>
                <a href="condi.html">Conditions générales</a>
                <a href="conf.html">Politique de confidentialité</a>
            </div>
            <div class="footer-column">
                <h3>Service client</h3>
                <a href="Ret.html">Contactez-nous</a>
            </div>
            <div class="footer-column">
                <h3>Newsletter</h3>
                <p>Abonnez-vous pour recevoir nos offres exclusives.</p>
                <form class="newsletter-form">
                    <input type="email" placeholder="Votre email" required>
                    <button type="submit" class="btn">S'abonner</button>
                </form>
            </div>
        </div>
        <div class="copyright">
            <p>&copy; 2024 BAMBYLOVE. Tous droits réservés.</p>
        </div>
    </footer>
    
    <script>
        // Fonction pour Wave
        function payWithWave() {
            const phone = "773767317"; // Remplacez par votre numéro Wave
            const amount = prompt("Entrez le montant (FCFA):", "5000");
            
            if (amount) {
                // Essaie d'ouvrir l'application Wave
                window.location.href = `wave://send?phone=${phone}&amount=${amount}`;
                
                // Solution de secours si le lien échoue
                setTimeout(() => {
                    alert(`Ouvrez l'application Wave et envoyez ${amount}FCFA au ${phone}\nRéférence: CMD${Date.now()}`);
                }, 500);
            }
        }

        // Fonction pour Orange Money
        function payWithOrange() {
            const amount = prompt("Entrez le montant (FCFA):", "5000");
            if (amount) {
                const codeUSSD = `*144*5*1*${amount}*12345%23`; // %23 = #
                window.location.href = `tel:${codeUSSD}`;
            }
        }
    </script>
</body>
</html>
