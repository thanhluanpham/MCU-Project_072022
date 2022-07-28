# MCU_Project_072022
facing issue 
	pSPIHandle->pSPI->CR1=tempreg; // is call for turn on bit 2 of SPI1_CR but it's not set due wrong address mapping in header file
    
    #define SPI1_BASEADDR (APB1PERIPH_BASE+0x3000U) //SPI_1 -> correct #define SPI1_BASEADDR (APB2PERIPH_BASE+0x3000U) //SPI_1

