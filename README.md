# UJNoticesApp — UJ Campus Notices

> A lightweight React Native mobile noticeboard application empowering University of Johannesburg students to view real-time campus announcements and retain access via offline-first local storage cache streams.

---

## Overview

**UJNoticesApp** is a mobile application built exclusively for students of the **University of Johannesburg**. The platform bridges the gap between students and campus announcements by providing a centralized, offline-friendly mobile workspace to:

* **View dynamic announcement streams** fetched directly from external online REST API servers.
* **Retain complete notice records** locally on the handset device to preserve access during connectivity dropouts.
* **Stay informed** cleanly via official UJ corporate signature layouts optimized for enhanced readability.

> This application implements a strict offline-first structural design framework. Announcements successfully loaded during active internet cycles remain permanently readable even when moving between lecture halls, basements, or areas with unstable campus Wi-Fi.

---

## Features

### Dynamic Live Sync Feeds
* **Native JavaScript Data Requests:** Natively connects to external training REST servers asynchronously using standard fetch implementations.
* **Data Slicing Constraints:** Automatically limits incoming notification arrays to display exactly the top 10 most recent records.
* **Visual Status Feedbacks:** Houses smooth loading indicator wheels and explicit, non-technical failure warning message components.

### Offline Cache Preservation
* **Local Handset Database Store:** Utilizes long-term AsyncStorage memory arrays to persist data arrays directly to the system partition.
* **Namespaced Domain Mapping:** Enforces clear separation variables using target keys (`@uj/notices/cache` and `@uj/notices/lastUpdated`).
* **Safe Target Space Clearance:** Built-in flush functions to erase assignment paths safely without breaking neighboring handset databases.
