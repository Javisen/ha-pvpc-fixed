# PVPC Hourly Pricing (Fixed by Javisen)

Este repositorio es un **fix temporal** para la integración de precios horários de electricidad en España (PVPC) de Home Assistant.

> [!IMPORTANT]
> **LEER ANTES DE INSTALAR**: Para evitar conflictos de entidades, es imprescindible desinstalar cualquier versión previa de la integración PVPC y reiniciar Home Assistant antes de proceder con esta instalación.
> 

### 🛠️ ¿Qué incluye este fix?
- **Corrección de festivos:** Se han actualizado manualmente los calendarios de festivos nacionales para los años **2026, 2027 y 2028**. Esto asegura que la tarifa P3 (Valle) se aplique correctamente durante todo el día en las fechas correspondientes.
- **Mantenimiento temporal:** Esta versión se mantendrá activa de forma provisional hasta que el desarrollador oficial actualice la integración original o se resuelvan los problemas de descarga de datos.

### ⚙️ Instalación
1. Añade este repositorio como **Repositorio Personalizado** en HACS.
2. Busca "PVPC fix Javisen)" e instala.
3. Reinicia Home Assistant.

# PVPC Hourly Pricing (Fixed by Javisen)

---

This is a **temporary fix** for the Spanish Electricity Hourly Pricing (PVPC) integration in Home Assistant. 

Due to the lack of recent updates in the official integration regarding holiday calendars, this fork provides a manual update to ensure the correct application of electricity tariffs.

### 🛠️ Key Improvements
- **Extended Holiday Support:** Manually updated the national holiday calendars for **2026, 2027, and 2028**.
- **Accurate Billing:** Ensures that the **P3 (Valley)** period is correctly applied 24h during national holidays, preventing incorrect cost calculations.
- **Continuous Maintenance:** This repository will remain active until the official integration or the underlying `aiopvpc` library is fully updated by the original maintainers.

### ⚙️ Installation via HACS
1. Open **HACS** in your Home Assistant instance.
2. Click on the three dots in the top right corner and select **Custom repositories**.
3. Paste the following URL: `https://github.com/Javisen/ha-pvpc-fixed`
4. Select **Integration** as the category and click **Add**.
5. Find "PVPC fix Javisen)" in the HACS list and click **Download**.
6. **Restart** Home Assistant to apply changes.

### 📝 Configuration
After restarting, go to **Settings** > **Devices & Services** > **Add Integration** and search for **PVPC**.
