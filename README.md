# Marketplace Project Hecto

## **Overview**
This is a fully functional e-commerce marketplace built with Next.js 14, TypeScript, Tailwind CSS, and Sanity CMS. The project integrates dynamic routes, responsive design, and a robust backend powered by Sanity CMS. 

The application is deployed on Vercel with a staging environment set up for testing and validation.

---

## **Features**
- **Product Listing**: Displays all products fetched from Sanity CMS.
- **Cart Functionality**: Add, remove, and update cart items.
- **Search and Filter**: Search bar and category filters to refine product lists.
- **Responsive Design**: Optimized for desktop and mobile devices.
- **Secure Environment Variables**: Managed securely using `.env` files and Vercel.

---

## **Deployment**
### **Staging Environment**
- **Platform**: Vercel
- **Environment Variables**:
  - NEXT_PUBLIC_SANITY_PROJECT_ID
  - NEXT_PUBLIC_SANITY_DATASET
  - SANITY_TOKEN
  - API_KEY

---

## **Tech Stack**
- **Frontend**: Next.js, TypeScript, Tailwind CSS
- **Backend**: Sanity CMS
- **Hosting**: Vercel
- **Testing Tools**: Cypress, Lighthouse, Postman

---

## **Folder Structure**
```
.
├── src/
│   ├── components/   # Reusable components
│   ├── pages/        # Dynamic routes
│   ├── utils/        # Utility functions
├── public/           # Static assets
├── documents/        # Reports and documentation
├── .env.local        # Environment variables (local)
├── README.md         # Project README
```

---

## **Testing**
### **Functional Testing**
- Verified workflows including product listing, cart functionality, and API interactions.

### **Performance Testing**
- Tools: Lighthouse
- Scores:
  - Performance: **96%**
  - Accessibility: **90%**
  - SEO: **100%**

### **Security Testing**
- Ensured secure API key handling and validated HTTPS.

---

## **How to Run Locally**
1. Clone the repository:
   ```bash
   git clone https://github.com/Akber261986/hackathon-ecommerce-web-q2.git
   ```
2. Navigate to the project directory:
   ```bash
   cd project-directory
   ```
3. Install dependencies:
   ```bash
   npm install
   ```
4. Add a `.env.local` file with the following:
   ```plaintext
   NEXT_PUBLIC_SANITY_PROJECT_ID=your_project_id
   NEXT_PUBLIC_SANITY_DATASET=production
   API_KEY=your_api_key
   ```
5. Run the development server:
   ```bash
   npm run dev
   ```
6. Open `http://localhost:3000` in your browser.

---

## **License**
This project is licensed under the MIT License. See the LICENSE file for details.

---

## **Contributing**
Contributions are welcome! Please open an issue or submit a pull request for any changes.

---

## **Acknowledgments**
- [Sanity CMS](https://www.sanity.io/)
- [Vercel](https://vercel.com/)
- [Next.js Documentation](https://nextjs.org/docs)
- [Tailwind CSS](https://tailwindcss.com/docs)