import streamlit as st
import numpy as np
import pandas as pd


def main():  
    st.title("Welcome to the Subject Specific Krishi Input Subsidy Scheme")  
    
    # Create radio buttons for navigation in the sidebar  
    option = st.sidebar.radio(  
        "Select a section:",  
        ("Introduction", "Organizational Chart", "Scope and Objectives")  
    )  

    # Call the corresponding function based on the selected option  
    if option == "Introduction":  
        introduction()  
    elif option == "Organizational Chart":  
        organizational_chart()  
    elif option == "Scope and Objectives":  
        scope_and_objectives()  

def introduction():  
    st.header("Introduction")  
    st.markdown("""  
    <div style='text-align: justify;'>  
        This is the introduction section of the application. Here, you will find information about the purpose and   
        features of the application. The goal is to provide users with a seamless experience and access to relevant   
        information without any hassle. The application is designed to be user-friendly and intuitive, making navigation   
        simple and efficient.  
    </div>  
    """, unsafe_allow_html=True)  

def organizational_chart():  
    st.header("Organizational Chart")  
    st.markdown("""  
    <div style='text-align: justify;'>  
        This section displays the organizational chart of the company. Direct Benefit Transfer (DBT) is a major   
        reform initiative to ensure transfer of benefits like wage payments, different types of subsidies, etc.,   
        directly to the bank accounts of the beneficiaries. This method not only reduces leakages but also ensures   
        timely delivery of benefits, enhancing the overall efficiency of welfare initiatives.  
    </div>  
    """, unsafe_allow_html=True)  

def scope_and_objectives():  
    st.header("Scope and Objectives")  
    st.markdown("""  
    <div style='text-align: justify;'>  
        This section outlines the scope and objectives of the project. It aims to define the boundaries of the   
        project and outline the main goals. By clearly stating objectives, we can ensure that all stakeholders   
        are aligned and working towards the same outcomes, improving collaboration and effectiveness.  
    </div>  
    """, unsafe_allow_html=True)  

if __name__ == "__main__":  
    main()
