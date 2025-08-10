# Document Creation Tool

A modern, interactive web application for creating professional business documents with a guided wizard interface. Built with React, TypeScript, and Vite, this tool helps users generate various types of business documents including RFP responses, Statements of Work, Business Proposals, and Service Contracts.

## 🚀 Features

### Document Types
- **RFP Response** - Comprehensive responses to Request for Proposal documents
- **Statement of Work** - Detailed project scope and deliverables documentation
- **Business Proposal** - Professional business proposals for new opportunities
- **Service Contract** - Service agreements and contract terms

### Key Features
- **Guided Wizard Interface** - Step-by-step document creation process
- **Rich Text Formatting** - Support for bold, italic, underline, colors, and font sizes
- **Content Block Selection** - Pre-built, customizable content blocks for different document sections
- **Project Information Management** - Customer details, project overview, technical specifications
- **Pricing Table Integration** - Built-in pricing calculator with itemized costs
- **Multiple Export Formats** - Export to DOCX, PDF, and HTML formats
- **Document Preview** - Real-time preview of the generated document
- **Drag & Drop Interface** - Intuitive content organization
- **Responsive Design** - Works seamlessly on desktop and mobile devices

## 🛠️ Technology Stack

- **Frontend Framework**: React 18.3.1
- **Language**: TypeScript 5.5.3
- **Build Tool**: Vite 5.4.2
- **Styling**: Tailwind CSS 3.4.1
- **Document Generation**: 
  - `docx` - Microsoft Word document creation
  - `jspdf` - PDF generation
  - `html2canvas` - HTML to canvas conversion
- **Icons**: Lucide React
- **Drag & Drop**: React Beautiful DnD
- **Development Tools**: ESLint, PostCSS, Autoprefixer

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd New-Doc-Creation-Tool
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:5173` to view the application

## 🚀 Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint for code quality

## 📋 Usage Guide

### Step 1: Document Type Selection
Choose from four document templates:
- RFP Response
- Statement of Work
- Business Proposal
- Service Contract

### Step 2: Project Information
Fill in the project details including:
- Customer name and logo
- Project name and start date
- Project overview and technical specifications
- Pricing table with line items
- Hardware and services components
- Header and footer text

### Step 3: Content Blocks
Select and customize pre-built content blocks:
- **Introduction** - Company introductions and overviews
- **Requirements** - Technical and project management requirements
- **Methodology** - Project delivery approaches
- **Timeline** - Project schedules and milestones
- **Pricing** - Cost breakdowns and payment terms

### Step 4: Preview & Export
- Review the complete document in real-time
- Export in multiple formats:
  - **DOCX** - Microsoft Word format
  - **PDF** - Portable Document Format
  - **HTML** - Web-ready format

## 🏗️ Project Structure

```
src/
├── components/           # React components
│   ├── DocumentPreview.tsx      # Document preview component
│   ├── DocumentTypeSelector.tsx # Document type selection
│   ├── ProjectInfoForm.tsx      # Project information form
│   ├── TextBlockSelector.tsx    # Content block selection
│   └── WizardProgress.tsx       # Progress indicator
├── data/                # Mock data and templates
│   └── mockData.ts      # Document types and text blocks
├── types/               # TypeScript type definitions
│   └── index.ts         # Interface definitions
├── App.tsx              # Main application component
├── main.tsx             # Application entry point
└── index.css            # Global styles
```

## 🎨 Customization

### Adding New Document Types
Edit `src/data/mockData.ts` to add new document types:

```typescript
export const documentTypes: DocumentType[] = [
  {
    id: 'new-type',
    name: 'New Document Type',
    description: 'Description of the new document type',
    icon: 'IconName'
  }
];
```

### Adding New Content Blocks
Add new text blocks to the `textBlocks` array in `src/data/mockData.ts`:

```typescript
{
  id: 'new-block',
  title: 'New Content Block',
  content: 'Your content here',
  formattedContent: [
    { text: 'Formatted content', style: { bold: true, fontSize: 'lg' } }
  ],
  category: 'CategoryName',
  isSelected: false
}
```

## 🔧 Configuration

### Tailwind CSS
The project uses Tailwind CSS for styling. Configuration can be found in `tailwind.config.js`.

### Vite Configuration
Build and development settings are configured in `vite.config.ts`.

### TypeScript
TypeScript configuration is split between:
- `tsconfig.json` - Base configuration
- `tsconfig.app.json` - Application-specific settings
- `tsconfig.node.json` - Node.js environment settings

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📞 Support

For support and questions, please open an issue in the repository or contact the development team.

## 🔄 Version History

- **v0.0.0** - Initial release with core document creation functionality
  - Wizard-based interface
  - Multiple document types
  - Rich text formatting
  - Export capabilities

---

**Built with ❤️ using React, TypeScript, and Vite** 