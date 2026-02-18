# AIml

from enum import Enum
from typing import Dict

class MethodColumn(Enum):
    """Колонны (Способы обработки) - parent commun"""
    PRYAMOY = "Прямой способ"
    PEREVALKA_PLOHAYA = "Перевалка плохая" 
    PEREVALKA_HOROSHAYA = "Перевалка хорошая"
    PZR = "ПЗР"
    T30 = "30Т"
    P33 = "33П"
    ZAPRESH = "Запрещ"
    ANYA = "Аня"

class PriemSOR(MethodColumn):
    """Строка ПРИЕМ - coefficients réception"""
    PRYAMOY = 1.0
    PEREVALKA_PLOHAYA = -0.5
    PEREVALKA_HOROSHAYA = 0.2
    PZR = -0.6
    T30 = 0.9
    P33 = -0.4
    ZAPRESH = -0.5
    ANYA = 0.5

class VydachaSOR(MethodColumn):
    """Строка ВЫДАЧА - coefficients livraison"""
    PRYAMOY = 1.0
    PEREVALKA_PLOHAYA = -0.5
    PEREVALKA_HOROSHAYA = 0.2
    PZR = -0.6
    T30 = 0.9
    P33 = -0.4
    ZAPRESH = -0.5
    ANYA = 0.5

# Usage ultra-simple :
print(PriemSOR.PZR.value)           # -0.6 → "ПЗР"
print(PriemSOR.PZR.value_ru)        # "ПЗР"
print(VydachaSOR["Перевалка плохая"].value)  # -0.5

