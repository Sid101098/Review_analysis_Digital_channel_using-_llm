# Bank App Negative Review Analysis

## Overview

This project provides a comprehensive automated system for analyzing negative user reviews of the banking application. The system collects 1-2 star reviews from the Google Play Store and performs multi-layered analysis to identify common complaints, technical issues, and user experience problems.

## Project Description

The analysis tool uses multiple approaches to gather and process user feedback:
- Play Store review scraping with advanced fallback mechanisms
- AI-powered analysis using local Ollama models
- Statistical and keyword-based pattern recognition
- Comprehensive data visualization
- Automated report generation

The system is designed to work reliably even when facing common challenges like scraping restrictions or AI model unavailability.

## Features

### Data Collection
- Multiple scraping strategies with different sorting methods and regions
- Smart fallback to simulated review data when scraping fails
- Automatic duplicate removal and data cleaning
- Realistic banking app complaint simulation based on common patterns

### Analysis Methods
- AI analysis using local Ollama models (Llama2, Mistral, etc.)
- Keyword-based categorization of common issues
- Sentiment and pattern analysis
- Statistical analysis of review metrics

### Visualization
- Rating distribution charts
- Review length analysis
- Word clouds of common complaints
- Issue frequency charts
- Helpful vote distribution

### Output Generation
- CSV files with raw review data
- Detailed text analysis reports
- Multiple visualization charts
- Executive summaries and recommendations

## Installation Requirements

### Python Packages
- google-play-scraper
- ollama
- matplotlib
- seaborn
- wordcloud
- pandas
- requests

### External Dependencies
- Ollama (for AI analysis) - optional
- Internet connection (for Play Store access)

## Usage

### Basic Execution
Run the main analysis function to automatically:
1. Fetch app information from Play Store
2. Collect negative reviews (1-2 stars)
3. Perform comprehensive analysis
4. Generate visualizations and reports

### Customization Options
- Modify APP_ID to analyze different applications
- Adjust MAX_REVIEWS to change sample size
- Configure analysis depth and methods
- Customize output formats and locations

## Key Functions

### Data Collection Functions
- fetch_app_info_multiple_methods: Retrieves basic app information using multiple scraping libraries
- fetch_reviews_advanced: Implements sophisticated review scraping with multiple strategies
- manual_review_search: Generates realistic simulated reviews when scraping fails
- fetch_reviews_with_fallback: Main data collector with comprehensive fallback system

### Analysis Functions
- analyze_with_ollama_improved: AI-powered review analysis with retry mechanisms
- perform_keyword_analysis: Pattern-based issue categorization
- create_comprehensive_analysis: Visualization and statistical analysis
- manual_fallback_analysis: Complete manual analysis when automated methods fail

### Core Orchestration
- main_analysis: Central function that coordinates the entire analysis workflow

## Output Files

The system generates several output files:
- CSV files containing raw review data with timestamps
- Text reports with detailed analysis findings
- PNG charts and visualizations
- Executive summaries with key insights and recommendations

## Analysis Categories

The system categorizes issues into:
- Technical Problems: App crashes, performance issues, bugs
- Login and Authentication: Login failures, OTP issues, biometric problems
- Transaction Issues: Payment failures, transfer problems, balance discrepancies
- User Experience: Poor UI design, navigation difficulties, confusing interfaces
- Security Concerns: Permission issues, privacy concerns, authentication problems
- Functional Issues: Specific banking features not working properly

## Fallback Mechanisms

The system includes multiple layers of redundancy:
1. Primary: Real Play Store review scraping
2. Secondary: Simulated review data based on common banking app issues
3. Tertiary: Manual analysis with predefined issue categories

This ensures the analysis completes successfully even under challenging conditions.

## Use Cases

- Product management for identifying app improvement priorities
- Quality assurance for tracking technical issues
- Customer support for understanding common user frustrations
- Competitive analysis for benchmarking against other banking apps
- Development planning for prioritizing feature fixes and enhancements

## Technical Details

- Built with Python 3.7+
- Uses multiple scraping libraries for reliability
- Implements proper rate limiting and error handling
- Supports both local and cloud execution environments
- Modular design for easy customization and extension

## Limitations

- Play Store scraping may be limited by Google's restrictions
- AI analysis requires local Ollama installation
- Simulated data provides generalized insights rather than app-specific findings
- Regional availability may affect review collection

## Future Enhancements

- Integration with additional app stores
- Support for more AI model providers
- Real-time monitoring capabilities
- Advanced natural language processing
- Sentiment trend analysis over time
- Competitive comparison features

This tool provides valuable insights for anyone responsible for maintaining or improving the Bank of Maharashtra MahaMobile application, helping to prioritize development efforts based on actual user feedback and common pain points.
