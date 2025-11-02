# 🚀 Databricks Training: Oil & Gas Data Analysis with WellView Data

A comprehensive beginner-friendly training notebook for learning Databricks fundamentals through hands-on oil & gas data analysis using realistic WellView system data.

## 📋 Overview

This training provides a 1-hour guided introduction to Databricks, designed specifically for data professionals in the oil & gas industry. Through practical exercises with synthetic well production data, you'll learn essential Databricks skills while working with familiar industry datasets.

### 🎯 Training Duration
- **Total Time:** 1 hour
- **Format:** Self-paced interactive notebook
- **Level:** Beginner

## 🔧 Prerequisites

### Technical Requirements
- Access to a Databricks workspace
- An active Databricks cluster (8.x or higher recommended)
- Basic familiarity with Python or SQL
- Web browser (Chrome, Firefox, Safari, or Edge)

### Knowledge Requirements
- Basic understanding of data concepts
- Familiarity with oil & gas terminology is helpful but not required
- No prior Databricks experience necessary

## 📚 Training Content

### Section 1: Databricks Notebook Basics (10 minutes)
- Introduction to Databricks platform
- Understanding magic commands (`%sql`, `%python`, `%md`, `%sh`, `%fs`)
- Markdown documentation best practices
- Interactive exercises with solutions

### Section 2: Unity Catalog Setup (10 minutes)
- Three-level namespace (catalog.schema.table)
- Setting up personal training schemas
- Understanding data governance basics
- Hands-on catalog and schema creation

### Section 3: Generate WellView Training Data (10 minutes)
- Understanding oil & gas data structures
- API well number format
- Creating realistic well header data
- Generating production and completion records
- Working with Delta Lake tables

### Section 4: Data Cleansing Techniques (10 minutes)
- Identifying and removing duplicate records
- Data standardization methods
- Handling NULL values
- Quality validation checks
- Practical exercises with production data

### Section 5: Creating Data Products (15 minutes)
- Complex joins between tables
- Aggregation and window functions
- Creating summary tables
- Performance metrics calculation
- Building reusable data products

### Section 6: Visualizations (10 minutes)
- Creating bar charts for top producers
- Pie charts for formation analysis
- Scatter plots for correlation analysis
- Interactive dashboard components
- Best practices for data visualization

### Section 7: Best Practices & Key Takeaways (5 minutes)
- Code optimization techniques
- Performance tuning tips
- Documentation standards
- Next steps for continued learning

## 🎓 Learning Objectives

By completing this training, you will be able to:

✅ Navigate and use Databricks notebooks effectively  
✅ Work with Unity Catalog's three-level namespace  
✅ Create and manage Delta Lake tables  
✅ Generate and manipulate data using PySpark  
✅ Perform data cleansing and standardization  
✅ Build data products with complex joins and aggregations  
✅ Create interactive visualizations using `display()`  
✅ Apply Databricks best practices in your projects  

## 🚀 Getting Started

### 1. Import the Notebook
```python
# Option 1: Upload directly to Databricks workspace
# Navigate to Workspace > Import > Upload File

# Option 2: Import from URL (if hosted)
# Workspace > Import > URL > [paste notebook URL]
```

### 2. Attach to Cluster
- Open the notebook in Databricks
- Click "Connect" in the top right
- Select an available cluster or create a new one

### 3. Run Setup Cells
- Execute cells in Section 1 & 2 first
- These create your personal training schema
- Follow the TODO instructions for hands-on practice

### 4. Complete Exercises
- Look for `#TODO` comments for exercises
- Solutions are provided in cells marked with `SOLUTION`
- Practice modifying queries and code

## 🗂️ Data Model

The training uses three interconnected tables mimicking a WellView system:

### Well Headers Table
- **Purpose:** Master well information
- **Key Fields:** API number, well name, operator, location, formation
- **Record Count:** ~100 wells

### Production Data Table  
- **Purpose:** Monthly production volumes
- **Key Fields:** Oil (BBL), gas (MCF), water (BBL) production
- **Record Count:** ~3,600 monthly records

### Completion Data Table
- **Purpose:** Well completion and fracturing details  
- **Key Fields:** Completion date, lateral length, number of stages
- **Record Count:** ~100 completion records

## 💡 Key Concepts Covered

### Magic Commands
- `%sql` - Execute SQL queries
- `%python` - Run Python code
- `%md` - Render markdown documentation
- `%sh` - Execute shell commands
- `%fs` - File system operations

### PySpark Operations
- **Transformations:** `select()`, `filter()`, `groupBy()`, `join()`, `withColumn()`
- **Actions:** `display()`, `count()`, `collect()`, `write()`
- **Aggregations:** `sum()`, `avg()`, `max()`, `min()`, `count()`

### Delta Lake Features
- ACID transactions
- Time travel capabilities
- Schema evolution
- Performance optimizations (OPTIMIZE, Z-ORDER)

### Oil & Gas Metrics
- Barrels of Oil Equivalent (BOE)
- Gas-to-Oil Ratio (GOR)
- Water cut percentage
- Production decline analysis

## 📊 Sample Visualizations

The training includes creating various visualization types:
- **Bar Charts:** Top producing wells by BOE
- **Pie Charts:** Production distribution by formation
- **Scatter Plots:** Lateral length vs. production correlation
- **Time Series:** Production trends over time

## 🔗 Additional Resources

### Databricks Documentation
- [Databricks Documentation](https://docs.databricks.com)
- [PySpark API Reference](https://spark.apache.org/docs/latest/api/python)
- [Delta Lake Documentation](https://docs.delta.io)

### Oil & Gas Resources
- [API Well Number Format](https://www.oil-gas.state.co.us/General/Help/APD_DST_Format.pdf)
- [Production Metrics Guide](https://www.spe.org/en/)

### Related Training
- Databricks Academy Free Courses
- Delta Lake Deep Dive
- Unity Catalog Advanced Features
- MLflow for Oil & Gas Applications

## 🤝 Contributing

Contributions are welcome! Please feel free to submit pull requests with:
- Additional exercises
- Industry-specific examples
- Performance optimization tips
- Bug fixes or improvements

### How to Contribute
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This training material is provided as-is for educational purposes. Feel free to adapt and use in your organization's training programs.

## 👥 Authors & Acknowledgments

- Created for Databricks beginners in the oil & gas industry
- Synthetic data generation inspired by real WellView systems
- Special thanks to the Databricks community for best practices

## 🐛 Issues & Support

If you encounter any issues or have questions:
1. Check the inline TODO comments and solutions
2. Review the best practices section
3. Open an issue in this repository
4. Contact your Databricks administrator

## 📈 Version History

- **v1.0** (October 2025) - Initial release
  - Core training modules
  - WellView data generation
  - Visualization exercises
  - Best practices guide

## 🎉 Ready to Start?

Import the notebook into your Databricks workspace and begin your journey to mastering Databricks for oil & gas data analysis!

---

**Happy Learning!** 🎓 Remember to practice with your own datasets after completing the training to reinforce your new skills.
