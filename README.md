# Celebal_Week5_Assignment
This Python-based tool enables selective data migration by allowing users to choose specific tables and columns to transfer between databases. It supports SQLAlchemy-compatible databases, ensures data control, and is ideal for compliance, reduced data loads, and targeted migrations.

--Copy Data from Database to CSV, Parquet, and Avro File Formats--
# Database Export Formats: CSV, Parquet, and Avro

This project demonstrates how to export data from a relational database (like Oracle, PostgreSQL, MySQL) into multiple file formats for use in reporting, analytics, and ETL workflows.

## 📦 File Formats Supported
- CSV (broad compatibility)
- Parquet (optimized for analytics)
- Avro (compact with schema evolution)

## 🔧 Technologies
- Python
- Pandas
- SQLAlchemy
- Fastavro
- PyArrow

## 🚀 How to Run

### 1. Install dependencies
```bash
pip install -r requirements.txt

--Configure Schedule Trigger and Event Triggers to Automate the Pipeline Process--
# Automated Data Pipeline with Schedule and Event Triggers

This project demonstrates a Python-based data pipeline automation setup using both:
- ⏰ Schedule Triggers (e.g., run every day at 9AM)
- 🛎️ Event Triggers (e.g., run when a file arrives)

No cloud required — fully local and scriptable.

---

## 🔧 Features

- Schedule pipeline runs with `schedule`
- Watch for file arrival using `watchdog`
- Simulate DB update detection (optional)
- Export sample data to `CSV`

---

## 🚀 Getting Started

### 1. Install dependencies
```bash
pip install -r requirements.txt

--Copy All Tables from One Database to Another--
# Full Database Replication Tool (Schema + Data)

This tool dynamically copies all tables and their contents from a source database to a destination database using Python. It ensures schema and data consistency and is useful for:

- Database migration
- Environment sync (e.g., staging → prod)
- Backup or archiving

## 💡 Features
- Auto-detect all tables
- Replicate schema and data
- Works with any SQLAlchemy-compatible DB (Oracle, MySQL, PostgreSQL, etc.)
- Logs operations to `replication.log`

---

## 🚀 How to Use

### 1. Install dependencies
```bash
pip install -r requirements.txt

--Copy Selective Tables with Selective Columns from One Database to Another--
# Selective Data Migration Tool

This tool allows you to migrate only selected tables and columns from one database to another. It's designed for:

- Partial migrations
- Compliance-driven exports
- Performance-optimized backups

## 💡 Features
- Migrate only what you define (table + column-level)
- Compatible with any SQLAlchemy-supported DB (Oracle, PostgreSQL, MySQL, etc.)
- Automatically creates destination tables
- Logs each migration for auditability

---

## ⚙️ Configuration

Edit `config.py`:

```python
SOURCE_DB_URI = "oracle+cx_oracle://user:pass@host:port/service"
DEST_DB_URI   = "postgresql://user:pass@localhost:5432/targetdb"

TABLES_TO_MIGRATE = {
    "employees": ["emp_id", "first_name", "last_name", "email"],
    "departments": ["dept_id", "dept_name"]
}
