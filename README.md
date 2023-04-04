# course-
animation d'un personnage qui courre
#include <iostream>
#include <chrono> // pour la fonction sleep

int main() {
    // Boucle infinie pour simuler l'animation de course
    while (true) {
        // Étape 1 : pied droit en avant
        std::cout << "    o/" << std::endl;
        std::cout << "   /|" << std::endl;
        std::cout << "   / \\" << std::endl;
        std::cout << "Pied droit en avant" << std::endl;
        std::this_thread::sleep_for(std::chrono::milliseconds(200)); // Pause de 200 millisecondes

        // Étape 2 : pied gauche en avant
        std::cout << "    \\o" << std::endl;
        std::cout << "    |\\" << std::endl;
        std::cout << "   / \\" << std::endl;
        std::cout << "Pied gauche en avant" << std::endl;
        std::this_thread::sleep_for(std::chrono::milliseconds(200)); // Pause de 200 millisecondes
    }

    return 0;
}
